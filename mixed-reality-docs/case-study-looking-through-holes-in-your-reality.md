---
title: 導入事例 - 実際には、セキュリティ ホールを見る
description: このケース スタディでは、ユーザーが、床下と実際の環境内の仮想の開口部には壁の後ろに表示できるように、HoloLens の「マジック ウィンドウ」効果を実装する方法について説明します。
author: EricRehmeyer
ms.author: ericrehm
ms.date: 03/21/2018
ms.topic: article
keywords: Windows Mixed Reality、HoloLens、マジックのウィンドウで、視差効果
ms.openlocfilehash: 0c0828a6ebbefdcff7f0a66f48469007c5c532df
ms.sourcegitcommit: 384b0087899cd835a3a965f75c6f6c607c9edd1b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/12/2019
ms.locfileid: "59600751"
---
# <a name="case-study---looking-through-holes-in-your-reality"></a>導入事例 - 実際には、セキュリティ ホールを見る

ユーザーは、複合現実と Microsoft HoloLens で実行できることを考えて、ときに、通常を引き続き使用質問などの「オブジェクト、ルームに追加できますか」。 または「どのようなことはレイヤー自分のスペースの上にでしょうか。」 検討するもう 1 つの部分を強調表示したい-基本的にマジック — にまたは周囲の実際の物理オブジェクトを検索するのと同じテクノロジを使用して。

## <a name="the-tech"></a>技術者

壁面を克服するように、エイリアンした試合かどうか **[RoboRaid](https://www.youtube.com/watch?v=Hf9qkURqtbM)**、壁に安全にロックを解除**[フラグメント](case-study-creating-an-immersive-experience-in-fragments.md)**、運が発生しました。UNSC 無限大格納庫を表示する、  **[E3 2015 で Halo 5 経験](https://www.youtube.com/watch?v=QDw5QjDtFy8)**、話の内容を見ています。 想像力に応じて、drywall に一時的なセキュリティ ホールを配置するか、loose floorboard 下の世界を非表示に、このビジュアルのトリックを使用できます。

![3 次元のパイプとその他の構造は、壁、侵入者を克服するように作成されたホールによってのみ表示 RoboRaid を追加します。](images/roboraid-640px.png)

3 次元のパイプとその他の構造は、壁、侵入者を克服するように作成されたホールによってのみ表示 RoboRaid を追加します。

HoloLens の一意のホログラムはこれらのいずれかを使用して、アプリは、同様の現実は実際のウィンドウを表示しますまたは、床、壁の背後にあるコンテンツの錯覚を提供できます。 左、自分で移動しが右側にあるを参照してください。 、近づくし、すべての複数のビットを確認できます。 主な違いは、実際の穴ことが許可される、を通じて、フロアがシリアルすることはできません holographic 魔法のようなコンテンツに上昇中です。 (は、タスク バックログを追加します、。)

## <a name="behind-the-scenes"></a>しくみ

この方法は、2 つの効果の組み合わせです。 まず、holographic のコンテンツが「空間のアンカー」を使用して、世界中にピン留め アンカーを使用することでそのコンテンツを「world ロック」することで表示されているが視覚的にドリフト近くに、物理オブジェクトから移動した場合や、基になる空間マッピング システムの部屋の 3D モデルを更新してを意味します。

第二に、holographic コンテンツは、のみ、実際には、穴を確認できるように、非常に特定の領域に視覚的に制限されます。 そのオクルー ジョン論理穴、ウィンドウ、または、トリックを販売するには、ドアを検索を要求する必要があります。 ビューのほとんどをブロックしているものシークレット ジュラシック ディメンションへの領域でのクラック可能性があります適切に配置された恐竜のようになりますだけです。

![これはなく実際のスクリーン ショット、HoloLens 上 MR 基本 101 からシークレット黄泉の外観の例です。 黒のエンクロージャは表示しませんが、仮想穴経由でコンテンツを確認できます。 (実際のデバイスを検索、ときに、フロアに思えますがあっても存在しない場合、それ以上の距離にある対象に見られるので、さらに表示されなくなります。)](images/origamiholecomposited-640px.png)

これはなく実際のスクリーン ショット、方法を示してからシークレット黄泉、 [MR 基本 101](holograms-101.md) HoloLens で検索します。 黒のエンクロージャは表示しませんが、仮想穴経由でコンテンツを確認できます。 (実際のデバイスを検索、ときに、フロアに思えますがあっても存在しない場合、それ以上の距離にある対象に見られるので、さらに表示されなくなります。)

### <a name="world-locking-holographic-content"></a>Holographic のコンテンツを世界中のロック

Unity では、世界中のロックを維持する holographic のコンテンツの原因と WorldAnchor コンポーネントを追加するだけです。

```
myObject.AddComponent<WorldAnchor>();
```

WorldAnchor コンポーネントは、位置と回転の GameObject (したがって、階層内には、そのオブジェクトの下のもの) の近くにある物理オブジェクトに対して相対的な安定に保つために絶えず調整します。 コンテンツを作成するときは、この仮想の穴に中央揃え、オブジェクトのルート ピボットされているように作成します。 (位置と回転に若干の調整は非常に顕著になるオブジェクトのピボットが壁の深い場所にある場合は、および穴は非常に安定した見えない可能性があります。)

### <a name="occluding-everything-but-the-virtual-hole"></a>すべてが仮想の穴を occluding

これは、さまざまな方法は、壁に何が非表示にビューを選択的にブロックします。 最も簡単なものでは、HoloLens が完全に黒のオブジェクトが非表示に表示されることを意味する、付加的な表示を使用するという事実を利用します。 これを行う Unity で任意の特殊なシェーダーや材料コツを行わず、黒のマテリアルを作成し、コンテンツ ボックス オブジェクトに割り当てることだけです。 たくない場合 3D モデリングを行うように、いくつかの既定の 4 つのオブジェクトを使用し、それらを少し重複だけです。 このアプローチの欠点がいくつかが動作、ものを取得する最も簡単な方法は、後でそれをリファクタリングする可能性がある場合でも、優れたが低忠実度の作業の概念実証を取得します。

前述の「ブラック_ボックス」アプローチを 1 つの主な欠点は、も写真しないことです。 効果は、HoloLens の表示を最適に見える場合があります、床、壁の残ったものではなく黒の大きなオブジェクトが行うすべてのスクリーン ショットに表示されます。 この理由は物理ハードウェアとスクリーン ショット複合ホログラムと現実が異なります。 偽のいくつかの計算には、少し迂回しましょう.

*偽の数値演算警告!これらの番号と数式についてに何らかの正確なメトリックの要点を説明するものです。*

表示される内容 HoloLens 経由。

```
( Reality * darkening_amount ) + Holograms
```

表示される内容のスクリーン ショットやビデオ。

```
( Reality * ( 1 - hologram_alpha ) ) + Holograms * hologram_alpha
```

英語版。暗くなった現実 (サングラスを通じてなど) と任意の単純な組み合わせは、HoloLens を参照してくださいホログラム、アプリを表示することです。 スクリーン ショットを取得するとき、カメラの画像は、ピクセルあたりの透明度の値に従って、アプリのホログラムとブレンドされます。

この問題を回避する方法の 1 つでは、のみ、深度バッファーに書き込むし、その他のすべての非透過マテリアルに並べ替えを「ブラック_ボックス」マテリアルを変更します。 この例では、チェック アウト、 [GitHub、MixedRealityToolkit に WindowOcclusion.shader ファイル](https://github.com/Microsoft/MixedRealityToolkit-Unity/blob/htk_release/Assets/HoloToolkit/Common/Shaders/WindowOcclusion.shader)します。 ここで、該当する行がコピーされます。

```
"RenderType" = "Opaque"
"Queue" = "Geometry"
ColorMask 0
```

(「オフセット 50 で 100」に注意してください行が問題に対処する関連のない、おそらく合理的を除外するためです)。

そのような非表示のオクルー ジョン マテリアルを実装すると、アプリは次の表示にし、複合現実のスクリーン ショットでは適切なボックスを描画します。 ボーナス ポイントも非表示 (ピクセル単位) を描画するために巧妙な処理を実行して、さらにそのボックスのパフォーマンスを改善しようとすることができますが、雑草を実際に取得できるを通常は必要ありません。

![Unity を描画し、他のボックスの外側の部分を除くここではシークレット黄泉 MR 基本 101 からです。 黄泉のピボットが穴の維持、ボックスの中央に、実際の現場の基準としたできるだけ安定に注意してください。](images/underworld-occluded-640px.png)

ここからシークレット黄泉[MR 基本 101](holograms-101.md) Unity を描画し、他のボックスの外側の部分を除く。 黄泉のピボットが穴の維持、ボックスの中央に、実際の現場の基準としたできるだけ安定に注意してください。

## <a name="do-it-yourself"></a>自分で行う

HoloLens があるし、自分の効果を試したいですか。 無料の 3D のビューアー アプリをインストールして読み込むに最も簡単な (コーディングは不要) を行うことができますが、[ダウンロード the.fbx ファイルが GitHub で紹介した](https://github.com/Microsoft/HolographicAcademy/tree/CaseStudy-MagicWindow/MagicWindow)の部屋で花 pot モデルを表示します。 HoloLens にロードすることと、職場で錯覚を確認できます。 小規模の穴にのみ表示できること、モデルの前にしたら、-他のすべては表示されません。 その他の任意の辺からモデルを見るし、それはまったく表示されなくなります。 移動、回転、および 3D ビューアーのスケールのコントロールを使用して、いくつかのアイデアを生成する考えることができます、垂直方向の画面に対して仮想穴の位置します。

![Unity エディターでこのモデルの表示、flowerpot 周囲に大きな黒いボックスが表示されます。 HoloLens で、ボックスは表示されなくなります、マジック ウィンドウ有効する方法を提供します。](images/magicwindowflowerpotineditor.png)

Unity エディターでこのモデルの表示、flowerpot 周囲に大きな黒いボックスが表示されます。 HoloLens で、ボックスは表示されなくなります、マジック ウィンドウ有効する方法を提供します。

この手法を使用するアプリをビルドする場合は、チェック アウト、 [MR 基本の 101 チュートリアル](holograms-101.md)で、 [Mixed Reality Academy](academy.md)します。 第 7 章では、(上記の絵) として非表示の黄泉を表示する、フロアが急増で終わります。 誰のチュートリアルを退屈させる必要があるか。

ここでは、実行できるこのアイデア [次へ] の。
* 仮想穴内で対話型コンテンツを作成する方法と考えてください。 壁のいくつかの影響を与えるユーザーのも無理はこの方法を提供できるという意味が実際に向上します。
* 既知の領域にオブジェクトを表示する方法と考えてください。 たとえば、方法する holographic 穴コーヒー テーブルをできます、フロアをその下にあるを参照してくださいでしょうか。

## <a name="about-the-author"></a>執筆者紹介

<table style="border-collapse:collapse">
<tr>
<td style="border-style: none" width="60px"><img alt="Picture of Eric Rehmeyer" width="60" height="60" src="images/genericusertile.jpg"></td>
<td style="border-style: none"><b>Eric Rehmeyer</b><br>シニア ソフトウェア エンジニア @Microsoft</td>
</tr>
</table>

## <a name="see-also"></a>関連項目
* [MR 基礎 101:デバイスとの完全なプロジェクト](holograms-101.md)
* [座標系](coordinate-systems.md)
* [空間のアンカー](spatial-anchors.md)
* [空間マッピング](spatial-mapping.md)
