---
title: ビルボード処理と tag-along
description: 常に、ビルボード処理を持つオブジェクトを回転自体、ユーザーが直面します。
author: radicalad
ms.author: adlinv
ms.date: 03/21/2018
ms.topic: article
keywords: Windows Mixed Reality、ビルボードの処理、tag-along
ms.openlocfilehash: 8215b96aff1f3c2d43e959f04ad83d41ffd32b2a
ms.sourcegitcommit: 384b0087899cd835a3a965f75c6f6c607c9edd1b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/12/2019
ms.locfileid: "59603170"
---
# <a name="billboarding-and-tag-along"></a>ビルボード処理と tag-along

ビルボード処理は、複合現実でのオブジェクトに適用できる動作の概念です。 常に、ビルボード処理を持つオブジェクトを回転自体、ユーザーが直面します。 これはテキストで特に便利で、隠ぺいされたまたは読み取り不可は、ユーザーが移動する場合、(世界ロック)、ユーザーの環境での静的オブジェクトの配置場所のメニュー システムがそれ以外の場合あります。

![HoloLens 見た常に、ユーザーが直面しているメニュー システム](images/billboarding-fragments.gif)<br>
*HoloLens 見た常に、ユーザーが直面しているメニュー システム*

ユーザーの環境で有効になっているためのビルボードを持つオブジェクトを自由に回転できます。 また、設計に関する考慮事項によって 1 つの軸にも制限できます。 注意してください、ビルボードのオブジェクトがクリッピングまたはすぎるに配置されている場合、それ自体が、他のオブジェクトに近い、または HoloLens では、スキャン、サーフェスが近すぎます。 これを回避するには、ビルボード処理を有効になっている軸の回転したときに、オブジェクトが生じる、合計使用量について考えます。

## <a name="what-is-a-tag-along"></a>Tag-along とは何ですか。

Tag-along は、ビルボードのオブジェクトを含むホログラムに追加できる動作の概念です。 この操作は、head ロックされているコンテンツの効果を実現するためのより自然でわかりやすい方法です。 Tag-along オブジェクトは、ユーザーのビューを離れないしようとします。 これにより、自由に新機能も、直接ビュー外ホログラムを見ながらそれらの前面と対話するユーザー。

![HoloLens のピン パネルは tag-along の動作方法を示す優れた例です。](images/tagalong-1000px.jpg)<br>
*HoloLens [スタート] メニューは tag-along 動作を示す優れた例です。*

Tag-along オブジェクトでは、これらの動作方法を調整することができますをパラメーターがあります。 コンテンツは、ユーザーが各自の環境の周囲に移動中にまたは必要に応じて、ユーザーの行の見えないようにすることができます。 ユーザーが移動すると、コンテンツは、ビューの端をスライドさせて、ユーザーの周囲を超えないしよう、に応じてユーザーがどの程度の速度に移動がままに一時的に非表示コンテンツ。 ときに、ユーザーは gazes tag-along オブジェクトの方向より完全に入ったビュー。 コンテンツを常に「概要離れた」ため、ユーザーは、その内容はどのような方向を決して忘れないでくださいと考えてください。

追加のパラメーターは、ラバー バンドでユーザーの頭にアタッチされていると感じる tag-along オブジェクトを作成できます。 物理的に複数存在すると思われるので、オブジェクトへの重みを提供加速と減速をダンプします。 この spring 動作は、tag-along のしくみの正確なメンタル モデルの構築を手助けするアフォー ダンスです。 オーディオは、ユーザーがオブジェクト tag-along モードの場合は、追加アフォーを提供します。 オーディオが; の動きの速度を再確認する必要があります。高速ヘッドには、自然な速度で処理する必要がありますが存在する場合は、オーディオ効果を最小限に顕著なサウンド効果を提供します。

コンテンツの真の head ロックと同様、tag-along オブジェクトは過負荷または nauseating 大きく移動またはスプリング ユーザーのビューが多すぎる場合を証明できます。 次のユーザーとし、すばやく、停止、感覚を伝えて停止しました。 残高は、自分の頭を停止しているオンにすると、視覚認識、世界の停止にすることをことを通知します。 ただしで維持 tag-along を移動するは、ユーザーが停止した場合、これが、感覚混乱します。

## <a name="see-also"></a>関連項目
* [カーソル](cursors.md)
* [相互作用の基礎](interaction-fundamentals.md)
* [快適性](comfort.md)
