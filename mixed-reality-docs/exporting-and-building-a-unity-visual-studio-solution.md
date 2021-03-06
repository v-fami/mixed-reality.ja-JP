---
title: エクスポートして、Unity Visual Studio ソリューションを構築します。
description: この記事では、複合現実プロジェクトをビルドし、Visual Studio でデプロイできるように Unity からエクスポートします。
author: ''
ms.author: mazeller
ms.date: 03/21/2018
ms.topic: article
keywords: unity では、visual studio は、エクスポート、ビルド、展開.
ms.openlocfilehash: 68c86fdfe0e589536dafe2bf53c7d4e5dffcc514
ms.sourcegitcommit: 384b0087899cd835a3a965f75c6f6c607c9edd1b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/12/2019
ms.locfileid: "59603698"
---
# <a name="exporting-and-building-a-unity-visual-studio-solution"></a>エクスポートして、Unity Visual Studio ソリューションを構築します。

使用するという推奨設定は、システムのキーボードを使用して、アプリケーションでの予定がない場合*D3D*アプリケーションが若干低いメモリを使用し、わずかに高速起動時間があります。 システムのキーボードを使用して、プロジェクトで TouchScreenKeyboard API を使用する場合は、としてエクスポートする必要があります。 *XAML*します。

## <a name="how-to-export-from-unity"></a>Unity からエクスポートする方法

![Unity ビルド設定](images/unitybuildsettings-300px.png)<br>
*Unity ビルド設定*

1. Unity からプロジェクトをエクスポートする準備ができたら、開く、**ファイル**メニュー選択し、**ビルド設定しています.**
2. クリックして**開くシーンを追加**ビルドにシーンを追加します。
3. **Build Settings**ダイアログ ボックスで、HoloLens をエクスポートする次のオプションを選択します。
   * **プラットフォーム:***ユニバーサル Windows プラットフォーム*を必ず選択して**スイッチ プラットフォーム**選択を有効にします。
   * **SDK:***ユニバーサル 10*します。
   * **UWP のビルドの種類:***D3D*します。
4. **省略可能な**:**UnityC#プロジェクト。** チェックされています。

>[!NOTE]
>このボックスをオンすることができます。
>* Visual Studio リモート デバッガーでアプリケーションをデバッグします。
>* Unity でスクリプトを編集C#WinRT Api を IntelliSense を使用しながらプロジェクト。

5. **ビルド設定しています.** ウィンドウを開いて、**プレーヤー設定しています.**
6. 選択、**ユニバーサル Windows プラットフォームの設定**タブ。
7. 展開、 **XR 設定**グループ。
8. **XR 設定** セクションで、チェック、**仮想現実サポート**新しいを追加するチェック ボックスをオン**仮想現実デバイス**ボックスの一覧を確認します **"Windows 混在実際には"** サポートされているデバイスとして表示されます。
9. 戻り、 **Build Settings**ダイアログ。
10. 選択**ビルド**します。
11. Windows エクスプ ローラー ダイアログ ボックスが表示される Unity のビルド出力を格納する新しいフォルダーを作成します。 一般に、名前、フォルダーの"App"を付けます。
12. 新しく作成したフォルダーを選択し、クリックして**フォルダーの選択**します。
13. Unity のビルドが完了すると、Windows エクスプ ローラー ウィンドウがプロジェクトのルート ディレクトリを開きます。 新しく作成したフォルダーに移動します。
14. このフォルダー内にある生成された Visual Studio ソリューション ファイルを開きます。

## <a name="when-to-re-export-from-unity"></a>Unity から再エクスポートします。

チェック、"C#プロジェクト"チェック ボックスを Unity からアプリをエクスポートする Visual Studio のソリューションを作成すると、すべての Unity スクリプト ファイルが含まれています。 これにより、Unity から再エクスポートせずに、スクリプトで反復処理することができます。 ただし、スクリプトの内容を変更するだけは、プロジェクトを変更する場合は、Unity からエクスポートして再必要があります。 Unity から再エクスポートする必要がある回数のいくつかの例は次のとおりです。
* 追加し、[プロジェクト] タブで資産を削除します。
* [Inspector] タブの任意の値を変更します。
* 追加し、階層 タブからオブジェクトを削除します。
* Unity プロジェクト設定を変更します。

## <a name="building-and-deploying-a-unity-visual-studio-solution"></a>構築および Unity Visual Studio ソリューションを展開します。

構築とアプリの展開の残りの部分が行われます[Visual Studio](using-visual-studio.md)します。 Unity のビルド構成を指定する必要があります。 Unity の名前付け規則は、何を通常はご利用いただけますを Visual Studio で異なる場合があります。

|  構成  |  説明 | 
|----------|----------|
|  デバッグ  |  オフのすべての最適化と、プロファイラーが有効になっています。 スクリプトをデバッグするために使用します。 | 
|  マスタ  |  すべての最適化をオンにし、プロファイラーを無効にします。 アプリをストアに送信するために使用します。 | 
|  リリース  |  すべての最適化をオンにし、プロファイラーを有効にします。 アプリのパフォーマンスを評価するために使用します。 | 

上記のリストを生成する必要があります。 Visual Studio プロジェクトを原因となる一般的なトリガーのサブセットであるに注意してください。 一般に、Visual Studio 内からの .cs ファイルを編集しても、Unity 内から再生成するプロジェクトには必要ありません。

## <a name="troubleshooting"></a>トラブルシューティング

場合は、.cs ファイルの編集の認識されて、Visual Studio プロジェクトではいないことを確認することを確認します。"UnityC#プロジェクト"Unity のビルド メニューから VS プロジェクトを生成する場合はオンになっています。
