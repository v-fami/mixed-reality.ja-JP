---
title: アプリの品質基準
description: このドキュメントでは、複合現実アプリの品質に影響を与える主な理由について説明します。
author: cjdgit
ms.author: crderr
ms.date: 03/21/2018
ms.topic: article
keywords: アプリの品質基準、実際には、混合 mixed reality アプリ
ms.openlocfilehash: 8070a434be462a636b314527c59f299ca77fb6d4
ms.sourcegitcommit: 384b0087899cd835a3a965f75c6f6c607c9edd1b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/12/2019
ms.locfileid: "59602381"
---
# <a name="app-quality-criteria"></a><span data-ttu-id="97711-104">アプリの品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-104">App quality criteria</span></span>

<span data-ttu-id="97711-105">このドキュメントでは、複合現実アプリの品質に影響を与える主な理由について説明します。</span><span class="sxs-lookup"><span data-stu-id="97711-105">This document describes the top factors impacting the quality of mixed reality apps.</span></span> <span data-ttu-id="97711-106">次の情報を提供する各要素について</span><span class="sxs-lookup"><span data-stu-id="97711-106">For each factor the following information is provided</span></span>
* <span data-ttu-id="97711-107">概要 – の品質要因と重要な理由の簡単な説明です。</span><span class="sxs-lookup"><span data-stu-id="97711-107">Overview – a brief description of the quality factor and why it is important.</span></span>
* <span data-ttu-id="97711-108">デバイスによる影響 - Mixed Reality をウィンドウのデバイスの種類は影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="97711-108">Device impact - which type of Window Mixed Reality device is impacted.</span></span>
* <span data-ttu-id="97711-109">品質基準 – の品質要因を評価する方法。</span><span class="sxs-lookup"><span data-stu-id="97711-109">Quality criteria – how to evaluate the quality factor.</span></span>
* <span data-ttu-id="97711-110">– メソッドに、問題を計測 (またはエクスペリエンス) を測定する方法。</span><span class="sxs-lookup"><span data-stu-id="97711-110">How to measure – methods to measure (or experience) the issue.</span></span>
* <span data-ttu-id="97711-111">推奨事項のより優れたユーザー エクスペリエンスを提供する方法の概要。</span><span class="sxs-lookup"><span data-stu-id="97711-111">Recommendations – summary of approaches to provide a better user experience.</span></span>
* <span data-ttu-id="97711-112">リソース-関連する開発者とアプリのより優れたエクスペリエンスを作成すると便利であるデザイン リソース</span><span class="sxs-lookup"><span data-stu-id="97711-112">Resources – relevant developer and design resources that are useful to create better app experiences.</span></span>

## <a name="frame-rate"></a><span data-ttu-id="97711-113">フレーム レート</span><span class="sxs-lookup"><span data-stu-id="97711-113">Frame rate</span></span>

<span data-ttu-id="97711-114">フレーム レートはホログラムの安定性とユーザーの快適性の最初の柱です。</span><span class="sxs-lookup"><span data-stu-id="97711-114">Frame rate is the first pillar of hologram stability and user comfort.</span></span> <span data-ttu-id="97711-115">推奨されるターゲットの下のフレーム レートには、ホログラムちらついたり、エクスペリエンスの信憑性に悪影響を与えると、目の疲労が発生する可能性を表示することがあります。</span><span class="sxs-lookup"><span data-stu-id="97711-115">Frame rate below the recommended targets can cause holograms to appear jittery, negatively impacting the believability of the experience and potentially causing eye fatigue.</span></span> <span data-ttu-id="97711-116">Windows Mixed Reality イマーシブ ヘッドセットでのユーザー エクスペリエンスのターゲット フレーム レートは、60 Hz またはサポートする Windows Mixed Reality 互換性のある Pc に応じて 90 Hz のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="97711-116">The target frame rate for your experience on Windows Mixed Reality immersive headsets will be either 60Hz or 90Hz depending on which Windows Mixed Reality Compatible PCs you wish to support.</span></span> <span data-ttu-id="97711-117">HoloLens 先のフレーム レートは 60 Hz です。</span><span class="sxs-lookup"><span data-stu-id="97711-117">For HoloLens the target frame rate is 60Hz.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-118">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-118">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-119"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-119"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-120"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-120"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-121">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-121">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-122">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-122">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-123">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-123">Quality criteria</span></span>

|  <span data-ttu-id="97711-124">最高</span><span class="sxs-lookup"><span data-stu-id="97711-124">Best</span></span>  |  <span data-ttu-id="97711-125">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-125">Meets</span></span> |  <span data-ttu-id="97711-126">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-126">Fail</span></span> |
--- | --- | ---
| <span data-ttu-id="97711-127">アプリでは、一貫してターゲット デバイスの 2 つ目の (FPS) 目標あたりのフレーム数を満たしています。HoloLens; に 60 fps90 超 Pc; fpsメイン ストリームの Pc で 60 fps します。</span><span class="sxs-lookup"><span data-stu-id="97711-127">The app consistently meets frames per second (FPS) goal for target device: 60fps on HoloLens; 90fps on Ultra PCs; and 60fps on mainstream PCs.</span></span> | <span data-ttu-id="97711-128">アプリは、コア エクスペリエンスを妨げていない断続的なフレームのドロップまたは、FPS は一貫して目標より低いが、アプリのエクスペリエンスを妨げるありません。</span><span class="sxs-lookup"><span data-stu-id="97711-128">The app has intermittent frame drops not impeding the core experience; or FPS is consistently lower than desired goal but doesn’t impede the app experience.</span></span> | <span data-ttu-id="97711-129">アプリには、フレーム レートの平均が 10 秒ごとに以下のドロップが発生しました。</span><span class="sxs-lookup"><span data-stu-id="97711-129">The app is experiencing a drop in frame rate on average every ten seconds or less.</span></span> |

### <a name="how-to-measure"></a><span data-ttu-id="97711-130">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-130">How to measure</span></span>

* <span data-ttu-id="97711-131">リアルタイムのフレーム レートのグラフがを通じてによって提供される、 [Windows Device Portal](using-the-windows-device-portal.md#system-performance) 「システムのパフォーマンス」の下。</span><span class="sxs-lookup"><span data-stu-id="97711-131">A real-time frame rate graph is provided through by the [Windows Device Portal](using-the-windows-device-portal.md#system-performance) under "System Performance".</span></span>
* <span data-ttu-id="97711-132">開発のデバッグには、アプリにフレーム レートの診断カウンターを追加します。</span><span class="sxs-lookup"><span data-stu-id="97711-132">For development debugging, add a frame rate diagnostic counter into the app.</span></span> <span data-ttu-id="97711-133">サンプルのカウンターは、リソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="97711-133">See Resources for a sample counter.</span></span>
* <span data-ttu-id="97711-134">フレーム レートの低下は、頭を左右に移動することによって、アプリの実行中に、デバイスで発生することができます。</span><span class="sxs-lookup"><span data-stu-id="97711-134">Frame rate drops can be experienced in device while the app is running by moving your head from side to side.</span></span> <span data-ttu-id="97711-135">ホログラムちらつく移動の予期しない場合は、フレーム レートが低い、または安定性の面が原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="97711-135">If the hologram shows unexpected jittery movement, then low frame rate or the stability plane is likely the cause.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-136">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-136">Recommendations</span></span>

* <span data-ttu-id="97711-137">開発作業の開始時に、フレーム レート カウンターを追加します。</span><span class="sxs-lookup"><span data-stu-id="97711-137">Add a frame rate counter at the beginning of the development work.</span></span>
* <span data-ttu-id="97711-138">フレーム レートの低下が発生する変更を評価して、パフォーマンス バグとして適切に解決する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-138">Changes that incur a drop in frame rate should be evaluated and appropriately resolved as a performance bug.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-139">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-139">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-140">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-140">Documentation</span></span>

* [<span data-ttu-id="97711-141">複合現実のパフォーマンスを理解</span><span class="sxs-lookup"><span data-stu-id="97711-141">Understanding Performance for Mixed Reality</span></span>](understanding-performance-for-mixed-reality.md)
* [<span data-ttu-id="97711-142">ホログラム安定性とフレーム レート</span><span class="sxs-lookup"><span data-stu-id="97711-142">Hologram stability and framerate</span></span>](hologram-stability.md#frame-rate)
* [<span data-ttu-id="97711-143">資産のパフォーマンスの予算</span><span class="sxs-lookup"><span data-stu-id="97711-143">Asset performance budget</span></span>](asset-creation-process.md)
* [<span data-ttu-id="97711-144">Unity のパフォーマンスに関する推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-144">Performance recommendations for Unity</span></span>](performance-recommendations-for-unity.md)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-145">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-145">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-146">MRToolkit、FPS カウンターの表示</span><span class="sxs-lookup"><span data-stu-id="97711-146">MRToolkit, FPS counter display</span></span>](https://github.com/Microsoft/MixedRealityToolkit-Unity/blob/htk_release/Assets/HoloToolkit/Utilities/README.md)
* [<span data-ttu-id="97711-147">MRToolkit、シェーダー</span><span class="sxs-lookup"><span data-stu-id="97711-147">MRToolkit, Shaders</span></span>](https://github.com/Microsoft/MixedRealityToolkit-Unity/tree/htk_release/Assets/HoloToolkit/Utilities/Shaders)

#### <a name="external-references"></a><span data-ttu-id="97711-148">外部参照</span><span class="sxs-lookup"><span data-stu-id="97711-148">External references</span></span>

* [<span data-ttu-id="97711-149">Unity では、モバイル アプリケーションの最適化</span><span class="sxs-lookup"><span data-stu-id="97711-149">Unity, Optimizing mobile applications</span></span>](https://www.youtube.com/watch?v=j4YAY36xjwE)

## <a name="hologram-stability"></a><span data-ttu-id="97711-150">ホログラム安定性</span><span class="sxs-lookup"><span data-stu-id="97711-150">Hologram stability</span></span>

<span data-ttu-id="97711-151">安定したホログラムは、使いやすさと、アプリの信憑性を向上し、ユーザーの使いやすい表示エクスペリエンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="97711-151">Stable holograms will increase the usability and believability of your app, and create a more comfortable viewing experience for the user.</span></span> <span data-ttu-id="97711-152">ホログラム安定性の品質が適切なアプリの開発と (追跡) を理解するデバイスの機能の結果をその環境。</span><span class="sxs-lookup"><span data-stu-id="97711-152">The quality of hologram stability is a result of good app development and the device's ability to understand (track) its environment.</span></span> <span data-ttu-id="97711-153">フレーム レートが安定性の最初の柱の中、その他の要因の安定性を含む影響を与えることができます。</span><span class="sxs-lookup"><span data-stu-id="97711-153">While frame rate is the first pillar of stability, other factors can impact stability including:</span></span>

* <span data-ttu-id="97711-154">安定化平面の使用</span><span class="sxs-lookup"><span data-stu-id="97711-154">Use of the stabilization plane</span></span>
* <span data-ttu-id="97711-155">空間アンカーまでの距離</span><span class="sxs-lookup"><span data-stu-id="97711-155">Distance to spatial anchors</span></span>
* <span data-ttu-id="97711-156">Tracking</span><span class="sxs-lookup"><span data-stu-id="97711-156">Tracking</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-157">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-157">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-158"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-158"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-159"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-159"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-160">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-160">✔️</span></span></td><td style="text-align: center;"></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-161">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-161">Quality criteria</span></span>

|  <span data-ttu-id="97711-162">最高</span><span class="sxs-lookup"><span data-stu-id="97711-162">Best</span></span>  |  <span data-ttu-id="97711-163">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-163">Meets</span></span> |  <span data-ttu-id="97711-164">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-164">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-165">ホログラムが一貫して安定したが表示されます。</span><span class="sxs-lookup"><span data-stu-id="97711-165">Holograms consistently appear stable.</span></span> | <span data-ttu-id="97711-166">セカンダリのコンテンツは予期しない動きです。または、予期しない動きが全体的なアプリ エクスペリエンスを妨げるありません。</span><span class="sxs-lookup"><span data-stu-id="97711-166">Secondary content exhibits unexpected movement; or unexpected movement does not impede overall app experience.</span></span> | <span data-ttu-id="97711-167">フレームで主要なコンテンツには、予期せぬ動作が発生します。</span><span class="sxs-lookup"><span data-stu-id="97711-167">Primary content in frame exhibits unexpected movement.</span></span> |

### <a name="how-to-measure"></a><span data-ttu-id="97711-168">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-168">How to measure</span></span>

<span data-ttu-id="97711-169">While ソックスを着けずに、デバイスと、エクスペリエンスを表示します。</span><span class="sxs-lookup"><span data-stu-id="97711-169">While wearing the device and viewing the experience:</span></span>

* <span data-ttu-id="97711-170">サイド バイ サイドに頭を移動、ホログラムが予期しない動きを表示する場合、フレーム レートが低いまたは焦点面に安定性の面の不適切なアラインメントは考えられる原因になります。</span><span class="sxs-lookup"><span data-stu-id="97711-170">Move your head from side to side, if the holograms show unexpected movement then low frame rate or improper alignment of the stability plane to the focal plane is the likely cause.</span></span>
* <span data-ttu-id="97711-171">ホログラムや環境を移動、スイムレーンと jumpiness などの動作を探します。</span><span class="sxs-lookup"><span data-stu-id="97711-171">Move around the holograms and environment, look for behaviors such as swim and jumpiness.</span></span> <span data-ttu-id="97711-172">この種類のアニメーションは、空間アンカーに環境、または距離を追跡しないデバイスによる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="97711-172">This type of motion is likely caused by the device not tracking the environment, or the distance to the spatial anchor.</span></span>
* <span data-ttu-id="97711-173">大規模な場合、または複数ホログラムがフレームでは、安定化平面に起因揺れの可能性がありますが表示された場合、並列で、ヘッドの位置を移動中に、さまざまな深さでホログラム動作を観察します。</span><span class="sxs-lookup"><span data-stu-id="97711-173">If large or multiple holograms are in the frame, observe hologram behavior at various depths while moving your head position from side to side, if shakiness appears this is likely caused by the stabilization plane.</span></span>

### <a name="recomendations"></a><span data-ttu-id="97711-174">Recomendations</span><span class="sxs-lookup"><span data-stu-id="97711-174">Recomendations</span></span>

* <span data-ttu-id="97711-175">開発作業の開始時、フレーム レート カウンターを追加します。</span><span class="sxs-lookup"><span data-stu-id="97711-175">Add an frame rate counter at the beginning of the development work.</span></span>
* <span data-ttu-id="97711-176">安定化平面を使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-176">Use the stabilization plane.</span></span>
* <span data-ttu-id="97711-177">常に、アンカーの 3 つのメートル単位でアンカー ホログラムをレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="97711-177">Always render anchored holograms within 3 meters of their anchor.</span></span>
* <span data-ttu-id="97711-178">環境の適切な追跡のためのセットアップを確認します。</span><span class="sxs-lookup"><span data-stu-id="97711-178">Make sure your environment is setup for proper tracking.</span></span>
* <span data-ttu-id="97711-179">フレーム内でさまざまな焦点の深さのレベルでホログラムを回避するために、エクスペリエンスをデザインします。</span><span class="sxs-lookup"><span data-stu-id="97711-179">Design your experience to avoid holograms at various focal depth levels within the frame.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-180">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-180">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-181">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-181">Documentation</span></span>

* [<span data-ttu-id="97711-182">ホログラム安定性とフレーム レート</span><span class="sxs-lookup"><span data-stu-id="97711-182">Hologram stability and framerate</span></span>](hologram-stability.md#frame-rate)
* [<span data-ttu-id="97711-183">安定化平面を使用して、ケース スタディ</span><span class="sxs-lookup"><span data-stu-id="97711-183">Case study, Using the stabilization plane</span></span>](case-study-using-the-stabilization-plane-to-reduce-holographic-turbulence.md)
* [<span data-ttu-id="97711-184">複合現実のパフォーマンスを理解</span><span class="sxs-lookup"><span data-stu-id="97711-184">Understanding Performance for Mixed Reality</span></span>](understanding-performance-for-mixed-reality.md)
* [<span data-ttu-id="97711-185">Unity のパフォーマンスに関する推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-185">Performance recommendations for Unity</span></span>](performance-recommendations-for-unity.md)
* [<span data-ttu-id="97711-186">空間のアンカー</span><span class="sxs-lookup"><span data-stu-id="97711-186">Spatial anchors</span></span>](spatial-anchors.md)
* [<span data-ttu-id="97711-187">追跡エラーの処理</span><span class="sxs-lookup"><span data-stu-id="97711-187">Handling tracking errors</span></span>](coordinate-systems.md#handling-tracking-errors)
* [<span data-ttu-id="97711-188">フレームの静止した基準</span><span class="sxs-lookup"><span data-stu-id="97711-188">Stationary frame of reference</span></span>](coordinate-systems.md#stationary-frame-of-reference)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-189">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-189">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-190">MR コンパニオン キット、Kinect IPD</span><span class="sxs-lookup"><span data-stu-id="97711-190">MR Companion Kit, Kinect IPD</span></span>](https://github.com/Microsoft/MixedRealityCompanionKit/tree/master/KinectIPD)

## <a name="holograms-position-on-real-surfaces"></a><span data-ttu-id="97711-191">実際の画面上の位置をホログラム</span><span class="sxs-lookup"><span data-stu-id="97711-191">Holograms position on real surfaces</span></span>

<span data-ttu-id="97711-192">物理オブジェクト相互の関連配置するためのもの) であればホログラムのずれは、ホログラムと実際の非結合の明確に示しています。</span><span class="sxs-lookup"><span data-stu-id="97711-192">Misalignments of holograms with physical objects (if intended to be placed in relation to one another) is a clear indication of the non-union of holograms and real-world.</span></span> <span data-ttu-id="97711-193">配置の精度が、シナリオのニーズを基準とする必要があります。たとえば、一般的な表面の配置は、空間のマップを使用できますより正確な配置マーカーおよび調整のいくつかの使用が必要になります。</span><span class="sxs-lookup"><span data-stu-id="97711-193">Accuracy of the placement should be relative to the needs of the scenario; for example, general surface placement can use the spatial map, but more accurate placement will require some use of markers and calibration.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-194">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-194">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-195"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-195"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-196"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-196"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-197">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-197">✔️</span></span></td><td style="text-align: center;"></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-198">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-198">Quality criteria</span></span>

|  <span data-ttu-id="97711-199">最高</span><span class="sxs-lookup"><span data-stu-id="97711-199">Best</span></span>  |  <span data-ttu-id="97711-200">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-200">Meets</span></span> |  <span data-ttu-id="97711-201">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-201">Fail</span></span> |
--- | --- | ---
| <span data-ttu-id="97711-202">ホログラムは、通常は、センチメートルでインチの範囲の画面に揃えます。</span><span class="sxs-lookup"><span data-stu-id="97711-202">Holograms align to the surface typically in the centimeters to inches range.</span></span> <span data-ttu-id="97711-203">精度が向上する必要がある場合、アプリは、必要なアプリ仕様内のコラボレーションの効率的な方法を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-203">If more accuracy is required, the app should provide an efficient means for collaboration within the desired app spec.</span></span> | <span data-ttu-id="97711-204">該当なし</span><span class="sxs-lookup"><span data-stu-id="97711-204">NA</span></span> | <span data-ttu-id="97711-205">サーフェスの平面互換性に影響するか、float、画面から離れた場所に表示される、ホログラムが物理的なターゲット オブジェクトにアラインされていない表示されます。</span><span class="sxs-lookup"><span data-stu-id="97711-205">The holograms appear unaligned with the physical target object by either breaking the surface plane or appearing to float away from the surface.</span></span> <span data-ttu-id="97711-206">精度が必要な場合、ホログラムはシナリオの近接仕様を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-206">If accuracy is required, Holograms should meet the proximity spec of the scenario.</span></span> | 

### <a name="how-to-measure"></a><span data-ttu-id="97711-207">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-207">How to measure</span></span>

* <span data-ttu-id="97711-208">ホログラム空間のマップに配置されている必要がありますが大幅に float、画面の上下には表示されません。</span><span class="sxs-lookup"><span data-stu-id="97711-208">Holograms that are placed on spatial map should not appear to dramatically float above or below the surface.</span></span>
* <span data-ttu-id="97711-209">ホログラム正確な配置を必要とするには、何らかの形のマーカーと調整システム シナリオの要件に正確である必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-209">Holograms that require accurate placement should have some form of marker and calibration system that is accurate to the scenario's requirement.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-210">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-210">Recommendations</span></span>

* <span data-ttu-id="97711-211">空間のマップは、有効桁数が必要なサーフェスでオブジェクトを配置するために便利です。</span><span class="sxs-lookup"><span data-stu-id="97711-211">Spatial map is useful for placing objects on surfaces when precision isn’t required.</span></span>
* <span data-ttu-id="97711-212">最適な精度では、マーカーまたはポスターを最終的な調整をホログラムと Xbox コント ローラー (または一部手動の配置メカニズム) を設定するのに使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-212">For the best precision, use markers or posters to set the holograms and an Xbox controller (or some manual alignment mechanism) for final calibration.</span></span>
* <span data-ttu-id="97711-213">論理部分に非常に大規模なホログラムを分割し、画面には、各部分の配置を検討してください。</span><span class="sxs-lookup"><span data-stu-id="97711-213">Consider breaking extra-large holograms into logical parts and aligning each part to the surface.</span></span>
* <span data-ttu-id="97711-214">不適切なセット interpupilary 距離 (IPD) にホログラム配置も影響することができます。</span><span class="sxs-lookup"><span data-stu-id="97711-214">Improperly set interpupilary distance (IPD) can also effect hologram alignment.</span></span> <span data-ttu-id="97711-215">常に、ユーザーの IPD に HoloLens を構成します。</span><span class="sxs-lookup"><span data-stu-id="97711-215">Always configure HoloLens to the user's IPD.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-216">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-216">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-217">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-217">Documentation</span></span>

* [<span data-ttu-id="97711-218">空間マッピングの配置</span><span class="sxs-lookup"><span data-stu-id="97711-218">Spatial mapping placement</span></span>](spatial-mapping.md#placement)
* [<span data-ttu-id="97711-219">スキャン処理ルーム</span><span class="sxs-lookup"><span data-stu-id="97711-219">Room scanning process</span></span>](case-study-expanding-the-spatial-mapping-capabilities-of-hololens.md)
* [<span data-ttu-id="97711-220">空間アンカーのベスト プラクティス</span><span class="sxs-lookup"><span data-stu-id="97711-220">Spatial anchors best practices</span></span>](spatial-anchors.md#best-practices)
* [<span data-ttu-id="97711-221">追跡エラーの処理</span><span class="sxs-lookup"><span data-stu-id="97711-221">Handling tracking errors</span></span>](coordinate-systems.md#handling-tracking-errors)
* [<span data-ttu-id="97711-222">Unity での空間のマッピング</span><span class="sxs-lookup"><span data-stu-id="97711-222">Spatial mapping in Unity</span></span>](spatial-mapping-in-unity.md)
* [<span data-ttu-id="97711-223">Vuforia 開発の概要</span><span class="sxs-lookup"><span data-stu-id="97711-223">Vuforia development overview</span></span>](vuforia-development-overview.md)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-224">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-224">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-225">MR 空間 230:空間マッピング</span><span class="sxs-lookup"><span data-stu-id="97711-225">MR Spatial 230: Spatial mapping</span></span>](holograms-230.md)
* [<span data-ttu-id="97711-226">MR Toolkit、空間マッピング ライブラリ</span><span class="sxs-lookup"><span data-stu-id="97711-226">MR Toolkit, Spatial Mapping Libraries</span></span>](https://github.com/Microsoft/MixedRealityToolkit-Unity/blob/htk_release/Assets/HoloToolkit/SpatialMapping/README.md)
* [<span data-ttu-id="97711-227">MR コンパニオン キット、ポスターの調整のサンプル</span><span class="sxs-lookup"><span data-stu-id="97711-227">MR Companion Kit, Poster Calibration Sample</span></span>](https://github.com/Microsoft/MixedRealityCompanionKit/tree/master/PosterCalibrationSample)
* [<span data-ttu-id="97711-228">MR コンパニオン キット、Kinect IPD</span><span class="sxs-lookup"><span data-stu-id="97711-228">MR Companion Kit, Kinect IPD</span></span>](https://github.com/Microsoft/MixedRealityCompanionKit/tree/master/KinectIPD)

#### <a name="external-references"></a><span data-ttu-id="97711-229">外部参照</span><span class="sxs-lookup"><span data-stu-id="97711-229">External references</span></span>

* [<span data-ttu-id="97711-230">Lowes ケース スタディ、有効桁数の配置</span><span class="sxs-lookup"><span data-stu-id="97711-230">Lowes Case Study, Precision alignment</span></span>](https://www.youtube.com/watch?v=LceMdyKZ4PI)

## <a name="viewing-zone-of-comfort"></a><span data-ttu-id="97711-231">快適性のゾーンの表示</span><span class="sxs-lookup"><span data-stu-id="97711-231">Viewing zone of comfort</span></span>

<span data-ttu-id="97711-232">アプリ開発者のコントロールはコンテンツとホログラムをさまざまな深さで配置することでユーザーの目が収束できます。</span><span class="sxs-lookup"><span data-stu-id="97711-232">App developers control where users' eyes converge by placing content and holograms at various depths.</span></span> <span data-ttu-id="97711-233">HoloLens ソックスを着けずにユーザーは、2.0 m 鮮明な画像は HoloLens に表示されるため、光学距離約 2.0 m ユーザーから離れた場所に固定は維持するために常に可能になります。</span><span class="sxs-lookup"><span data-stu-id="97711-233">Users wearing HoloLens will always accommodate to 2.0m to maintain a clear image because HoloLens displays are fixed at an optical distance approximately 2.0m away from the user.</span></span> <span data-ttu-id="97711-234">不適切なコンテンツの階層レベルは、visual 不安や疲労につながることができます。</span><span class="sxs-lookup"><span data-stu-id="97711-234">Improper content depth can lead to visual discomfort or fatigue.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-235">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-235">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-236"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-236"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-237"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-237"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-238">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-238">✔️</span></span></td><td style="text-align: center;"></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-239">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-239">Quality criteria</span></span>

<table>
<tr>
<td> <span data-ttu-id="97711-240">最高</span><span class="sxs-lookup"><span data-stu-id="97711-240">Best</span></span> </td><td><ul>
<li><span data-ttu-id="97711-241">2 分には、コンテンツを配置します。</span><span class="sxs-lookup"><span data-stu-id="97711-241">Place content at 2m.</span></span></li><li><span data-ttu-id="97711-242">ホログラムは 2 m に配置されることはできず、収束と宿泊施設間の競合を回避することはできません、ホログラムを配置するための最適なゾーンが 1.25 m と 5 分間は。</span><span class="sxs-lookup"><span data-stu-id="97711-242">When holograms cannot be placed at 2m and conflicts between convergence and accommodation cannot be avoided, the optimal zone for hologram placement is between 1.25m and 5m.</span></span></li><li><span data-ttu-id="97711-243">すべてのケースでは、デザイナーがコンテンツを 1 以上の対話をユーザーに促すことを構成する必要がありますメートル離れた場所 (例: コンテンツのサイズを調整して、既定の配置パラメーター)。</span><span class="sxs-lookup"><span data-stu-id="97711-243">In every case, designers should structure content to encourage users to interact 1+ m away (e.g. adjust content size and default placement parameters).</span></span></li><li><span data-ttu-id="97711-244">具体的にはないシナリオで必要に応じて、しない限り、クリッピング平面が 1 m で始まる fadeout と実装にあります。</span><span class="sxs-lookup"><span data-stu-id="97711-244">Unless specifically not required by the scenario, a clipping plane should be implement with fadeout starting at 1m.</span></span></li><li><span data-ttu-id="97711-245">ようにホログラムの近くの監視が必要な場合は、コンテンツの 50 cm よりも近いしない場合があります。</span><span class="sxs-lookup"><span data-stu-id="97711-245">In cases where closer observation of a motionless hologram is required, the content should not be closer than 50cm.</span></span></li>
</ul></td>
</tr><tr>
<td> <span data-ttu-id="97711-246">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-246">Meets</span></span></td><td> <span data-ttu-id="97711-247">コンテンツは、内で、表示およびモーションのガイダンスが、不適切な使用またはクリップの平面は使用されていません。</span><span class="sxs-lookup"><span data-stu-id="97711-247">Content is within the viewing and motion guidance, but improper use or no use of the clipping plane.</span></span></td>
</tr><tr>
<td> <span data-ttu-id="97711-248">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-248">Fail</span></span> </td><td> <span data-ttu-id="97711-249">コンテンツの表示が近すぎる (通常&lt;1.25 m、または&lt;50 cm 静止ホログラムを詳しく監視を必要とするのです)。</span><span class="sxs-lookup"><span data-stu-id="97711-249">Content is presented too close (typically &lt;1.25m, or &lt;50cm for stationary holograms requiring closer observation.)</span></span></td>
</tr>
</table>

### <a name="how-to-measure"></a><span data-ttu-id="97711-250">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-250">How to measure</span></span>

* <span data-ttu-id="97711-251">コンテンツ通常は 2 m、退席中、1.25 または 5 分よりもさらにより近いいいえ。</span><span class="sxs-lookup"><span data-stu-id="97711-251">Content should typically be 2m away, but no closer than 1.25 or further than 5m.</span></span>
* <span data-ttu-id="97711-252">いくつかの例外を除き、HoloLens クリッピング レンダリングまでの距離を .85CM に fadeout 1 m からコンテンツを設定してください。</span><span class="sxs-lookup"><span data-stu-id="97711-252">With few exceptions, the HoloLens clipping render distance should be set to .85CM with fadeout of content starting at 1m.</span></span> <span data-ttu-id="97711-253">コンテンツのアプローチし、クリッピング平面の影響に注意してください。</span><span class="sxs-lookup"><span data-stu-id="97711-253">Approach the content and note the clipping plane effect.</span></span>
* <span data-ttu-id="97711-254">静止しているコンテンツを 50 cm 離れたよりも近いすることはできません。</span><span class="sxs-lookup"><span data-stu-id="97711-254">Stationary content should not be closer than 50cm away.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-255">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-255">Recommendations</span></span>

* <span data-ttu-id="97711-256">2 分の最適な表示距離のコンテンツをデザインします。</span><span class="sxs-lookup"><span data-stu-id="97711-256">Design content for the optimal viewing distance of 2m.</span></span>
* <span data-ttu-id="97711-257">コンテンツが 1 m で始まる fadeout と 85 cm クリッピング レンダリングまでの距離を設定します。</span><span class="sxs-lookup"><span data-stu-id="97711-257">Set the clipping render distance to 85cm with fadeout of content starting at 1m.</span></span>
* <span data-ttu-id="97711-258">近い場所を表示する必要がある静止ホログラム、30 cm 以内にないはクリップの面で、fadeout は少なくとも 10 cm クリッピング平面からを起動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-258">For stationary holograms that need closer viewing, the clipping plane should be no closer than 30cm and fadeout should start at least 10cm away from the clipping plane.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-259">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-259">Resources</span></span>

* [<span data-ttu-id="97711-260">距離をレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="97711-260">Render distance</span></span>](hologram-stability.md#hologram-render-distances)
* [<span data-ttu-id="97711-261">Unity でのフォーカス ポイント</span><span class="sxs-lookup"><span data-stu-id="97711-261">Focus point in Unity</span></span>](focus-point-in-unity.md)
* [<span data-ttu-id="97711-262">スケールみる</span><span class="sxs-lookup"><span data-stu-id="97711-262">Experimenting with scale</span></span>](scale.md#experimenting-with-scale)
* [<span data-ttu-id="97711-263">テキスト、フォント サイズの推奨</span><span class="sxs-lookup"><span data-stu-id="97711-263">Text, Recommended font size</span></span>](typography.md#recommended-font-size)

## <a name="depth-switching"></a><span data-ttu-id="97711-264">深さの切り替え</span><span class="sxs-lookup"><span data-stu-id="97711-264">Depth switching</span></span>

<span data-ttu-id="97711-265">快適性の問題のゾーンを表示に関係なくほぼし、oculomotor の疲労と一般的な不安をする可能性があります (ホログラムと実際のコンテンツを含む) までの焦点のオブジェクト間や頻繁にすばやくを切り替えるユーザーを要求します。</span><span class="sxs-lookup"><span data-stu-id="97711-265">Regardless of viewing zone of comfort issues, demands for the user to switch frequently or quickly between near and far focal objects (including holograms and real-world content) can lead to oculomotor fatigue, and general discomfort.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-266">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-266">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-267"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-267"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-268"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-268"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-269">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-269">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-270">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-270">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-271">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-271">Quality criteria</span></span>

|  <span data-ttu-id="97711-272">最高</span><span class="sxs-lookup"><span data-stu-id="97711-272">Best</span></span>  |  <span data-ttu-id="97711-273">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-273">Meets</span></span> |  <span data-ttu-id="97711-274">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-274">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-275">切り替えを限定的または自然の深さが原因で、ユーザーが膨らみます不自然しません。</span><span class="sxs-lookup"><span data-stu-id="97711-275">Limited or natural depth switching that doesn’t cause the user to unnaturally refocus.</span></span> | <span data-ttu-id="97711-276">これはコアであり、アプリのエクスペリエンスに組み込むの突然の深さスイッチ、または実際の予期しないコンテンツによって発生した突然深さスイッチ。</span><span class="sxs-lookup"><span data-stu-id="97711-276">Abrupt depth switch this is core and designed into the app experience, or abrupt depth switch that is caused by unexpected real-world content.</span></span> | <span data-ttu-id="97711-277">一貫性のある深さスイッチ、または深さの突然の切り替えは必要のないまたは core アプリのエクスペリエンスをします。</span><span class="sxs-lookup"><span data-stu-id="97711-277">Consistent depth switch, or abrupt depth switching that isn’t necessary or core to the app experience.</span></span> | 

### <a name="how-to-measure"></a><span data-ttu-id="97711-278">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-278">How to measure</span></span>

* <span data-ttu-id="97711-279">アプリが一貫してや突然の深さのフォーカスを変更するユーザーが必要な場合は、問題の切り替えの深さです。</span><span class="sxs-lookup"><span data-stu-id="97711-279">If the app requires the user to consistently and/or abruptly change depth focus, there is depth switching problem.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-280">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-280">Recommendations</span></span>

* <span data-ttu-id="97711-281">一貫性のある焦点面で主要なコンテンツを保持し、安定化の平面が焦点面と一致するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="97711-281">Keep primary content at a consistent focal plane and make sure the stabilization plane matches the focal plane.</span></span> <span data-ttu-id="97711-282">Oculomotor 疲労と予期しないホログラム移動が軽減されます。</span><span class="sxs-lookup"><span data-stu-id="97711-282">This will alleviate oculomotor fatigue and unexpected hologram movement.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-283">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-283">Resources</span></span>

* [<span data-ttu-id="97711-284">距離をレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="97711-284">Render distance</span></span>](hologram-stability.md#hologram-render-distances)
* [<span data-ttu-id="97711-285">Unity でのフォーカス ポイント</span><span class="sxs-lookup"><span data-stu-id="97711-285">Focus point in Unity</span></span>](focus-point-in-unity.md)

## <a name="use-of-spatial-sound"></a><span data-ttu-id="97711-286">空間のサウンドの使用</span><span class="sxs-lookup"><span data-stu-id="97711-286">Use of spatial sound</span></span>

<span data-ttu-id="97711-287">Windows Mixed Reality では、オーディオ エンジンは、3 D の方向、距離、および環境のシミュレーションを使用してサウンドをシミュレートすることで、複合現実エクスペリエンスの聴覚的なコンポーネントを提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-287">In Windows Mixed Reality, the audio engine provides the aural component of the mixed reality experience by simulating 3D sound using direction, distance, and environmental simulations.</span></span> <span data-ttu-id="97711-288">アプリケーションでサウンドの空間を使用すると、ユーザーを囲むが 3 次元空間 (球) でサウンドを配置する開発者ができます。</span><span class="sxs-lookup"><span data-stu-id="97711-288">Using spatial sound in an application allows developers to convincingly place sounds in a 3 dimensional space (sphere) all around the user.</span></span> <span data-ttu-id="97711-289">それらのサウンドは、実際の物理オブジェクトまたはユーザーの環境での複合現実ホログラムから送信されるがまるでようですが。</span><span class="sxs-lookup"><span data-stu-id="97711-289">Those sounds will then seem as if they were coming from real physical objects or the mixed reality holograms in the user's surroundings.</span></span> <span data-ttu-id="97711-290">サウンドの空間は、immersion、アクセシビリティ、および複合現実のアプリケーションでの UX デザインの強力なツールです。</span><span class="sxs-lookup"><span data-stu-id="97711-290">Spatial sound is a powerful tool for immersion, accessibility, and UX design in mixed reality applications.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-291">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-291">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-292"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-292"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-293"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-293"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-294">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-294">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-295">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-295">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-296">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-296">Quality criteria</span></span>

|  <span data-ttu-id="97711-297">最高</span><span class="sxs-lookup"><span data-stu-id="97711-297">Best</span></span>  |  <span data-ttu-id="97711-298">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-298">Meets</span></span> |  <span data-ttu-id="97711-299">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-299">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-300">サウンドが spatialized は論理的にし、適切に、UX はオブジェクトの検出とユーザーのフィードバックを支援するサウンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-300">Sound is logically spatialized, and the UX appropriately uses sound to assist with object discovery and user feedback.</span></span> <span data-ttu-id="97711-301">サウンドがシナリオ全体であり自然なオブジェクトに関連する正規化されました。</span><span class="sxs-lookup"><span data-stu-id="97711-301">Sound is natural and relevant to objects and normalized across the scenario.</span></span> | <span data-ttu-id="97711-302">空間オーディオは、信憑性で適切に使用されますが、ユーザーからのフィードバックと見つけやすさを支援するための手段として存在します。</span><span class="sxs-lookup"><span data-stu-id="97711-302">Spatial audio is used appropriately for believability but missing as means to help with user feedback and discoverability.</span></span> | <span data-ttu-id="97711-303">予想どおり、サウンドが spatialized いないや UX 内のユーザーを支援するために、サウンドの欠如</span><span class="sxs-lookup"><span data-stu-id="97711-303">Sound is not spatialized as expected, and/or lack of sound to assist user within the UX.</span></span> <span data-ttu-id="97711-304">または空間オーディオがないと見なされますまたはシナリオの設計で使用されます。</span><span class="sxs-lookup"><span data-stu-id="97711-304">Or spatial audio was not considered or used in the design of the scenario.</span></span> | 

### <a name="how-to-measure"></a><span data-ttu-id="97711-305">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-305">How to measure</span></span>

* <span data-ttu-id="97711-306">一般に、関連するサウンドがターゲット ホログラムから出力する必要があります (例:、holographic dog から見かけサウンド。)。</span><span class="sxs-lookup"><span data-stu-id="97711-306">In general, relevant sounds should emit from target holograms (eg., bark sound coming from holographic dog.)</span></span>
* <span data-ttu-id="97711-307">フィードバックや認識 holographic フレーム外のアクションのユーザーを支援するためには、ユーザー エクスペリエンス全体でサウンド キューを使用してください。</span><span class="sxs-lookup"><span data-stu-id="97711-307">Sound cues should be used throughout the UX to assist the user with feedback or awareness of actions outside the holographic frame.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-308">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-308">Recommendations</span></span>

* <span data-ttu-id="97711-309">空間オーディオを使用して、オブジェクトの検出とユーザー インターフェイスを支援します。</span><span class="sxs-lookup"><span data-stu-id="97711-309">Use spatial audio to assist with object discovery and user interfaces.</span></span>
* <span data-ttu-id="97711-310">サウンドの実際の作業が合成または不自然なサウンドよりも優れています。</span><span class="sxs-lookup"><span data-stu-id="97711-310">Real sounds work better than synthesize or unnatural sound.</span></span>
* <span data-ttu-id="97711-311">ほとんどのサウンドを spatialized する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-311">Most sounds should be spatialized.</span></span>
* <span data-ttu-id="97711-312">発信機を非表示をしないようにします。</span><span class="sxs-lookup"><span data-stu-id="97711-312">Avoid invisible emitters.</span></span>
* <span data-ttu-id="97711-313">空間のマスクを回避します。</span><span class="sxs-lookup"><span data-stu-id="97711-313">Avoid spatial masking.</span></span>
* <span data-ttu-id="97711-314">すべてのサウンドを正規化します。</span><span class="sxs-lookup"><span data-stu-id="97711-314">Normalize all sounds.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-315">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-315">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-316">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-316">Documentation</span></span>

* [<span data-ttu-id="97711-317">空間のサウンド</span><span class="sxs-lookup"><span data-stu-id="97711-317">Spatial sound</span></span>](spatial-sound.md)
* [<span data-ttu-id="97711-318">サウンドの空間の設計</span><span class="sxs-lookup"><span data-stu-id="97711-318">Spatial sound design</span></span>](spatial-sound-design.md)
* [<span data-ttu-id="97711-319">Unity での空間のサウンド</span><span class="sxs-lookup"><span data-stu-id="97711-319">Spatial sound in Unity</span></span>](spatial-sound-in-unity.md)
* [<span data-ttu-id="97711-320">ケース スタディ、HoloTour のサウンドの空間</span><span class="sxs-lookup"><span data-stu-id="97711-320">Case study, Spatial sound for HoloTour</span></span>](case-study-spatial-sound-design-for-holotour.md)
* [<span data-ttu-id="97711-321">RoboRaid でサウンドの空間を使用して、ケース スタディ</span><span class="sxs-lookup"><span data-stu-id="97711-321">Case study, Using spatial sound in RoboRaid</span></span>](case-study-using-spatial-sound-in-roboraid.md)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-322">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-322">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-323">MR 空間 220:空間のサウンド</span><span class="sxs-lookup"><span data-stu-id="97711-323">MR Spatial 220: Spatial sound</span></span>](holograms-220.md)
* [<span data-ttu-id="97711-324">MRToolkit、空間オーディオ</span><span class="sxs-lookup"><span data-stu-id="97711-324">MRToolkit, Spatial Audio</span></span>](https://github.com/Microsoft/MixedRealityToolkit-Unity/blob/htk_release/Assets/HoloToolkit/SpatialSound/README.md)

## <a name="focus-on-holographic-frame-fov-boundaries"></a><span data-ttu-id="97711-325">Holographic フレーム (FOV) の境界に集中します。</span><span class="sxs-lookup"><span data-stu-id="97711-325">Focus on holographic frame (FOV) boundaries</span></span>

<span data-ttu-id="97711-326">適切に設計されたユーザー エクスペリエンスを作成し、仮想環境、ユーザーの周りを拡張するのに便利なコンテキストを維持できます。</span><span class="sxs-lookup"><span data-stu-id="97711-326">Well-designed user experiences can create and maintain useful context of the virtual environment that extends around the users.</span></span> <span data-ttu-id="97711-327">コンテンツのスケールとコンテキストの親切なデザイン FOV 境界の影響を軽減する必要があります、空間オーディオ、ガイダンスのシステムとユーザーの位置を使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-327">Mitigating the effect of the FOV boundaries involves a thoughtful design of content scale and context, use of spatial audio, guidance systems, and the user's position.</span></span> <span data-ttu-id="97711-328">場合、ユーザーは快適なアプリ エクスペリエンスをことができますが、FOV 境界によって損なわれる小さいを感じです。</span><span class="sxs-lookup"><span data-stu-id="97711-328">If done right, the user will feel less impaired by the FOV boundaries while having a comfortable app experience.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-329">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-329">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-330"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-330"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-331"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-331"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-332">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-332">✔️</span></span></td><td style="text-align: center;"></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-333">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-333">Quality criteria</span></span>

|  <span data-ttu-id="97711-334">最高</span><span class="sxs-lookup"><span data-stu-id="97711-334">Best</span></span>  |  <span data-ttu-id="97711-335">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-335">Meets</span></span> |  <span data-ttu-id="97711-336">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-336">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-337">ユーザー コンテキストを失うことは、表示する使いやすい。</span><span class="sxs-lookup"><span data-stu-id="97711-337">User never loses context and viewing is comfortable.</span></span> <span data-ttu-id="97711-338">ラージ オブジェクトのコンテキストのサポートが提供されます。</span><span class="sxs-lookup"><span data-stu-id="97711-338">Context assistance is provided for large objects.</span></span> <span data-ttu-id="97711-339">フレームの外側のオブジェクトの見つけやすさとガイダンスの表示が提供されます。</span><span class="sxs-lookup"><span data-stu-id="97711-339">Discoverability and viewing guidance is provided for objects outside the frame.</span></span> <span data-ttu-id="97711-340">一般に、モーションの設計と、ホログラムの小数点以下桁数は、快適な表示エクスペリエンスに適しています。</span><span class="sxs-lookup"><span data-stu-id="97711-340">In general, motion design and scale of the holograms are appropriate for a comfortable viewing experience.</span></span> | <span data-ttu-id="97711-341">ユーザーには、コンテキストが失われることが、余分の足部の動きを限られた状況で必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-341">User never loses context, but extra neck motion may be required in limited situations.</span></span> <span data-ttu-id="97711-342">限られた状況では、スケールはホログラム ホログラムを表示するには、いくつかネック モーションの原因と垂直方向または水平方向のフレームのいずれかを中断するとします。</span><span class="sxs-lookup"><span data-stu-id="97711-342">In limited situations scale causes holograms to break either the vertical or horizontal frame causing some neck motion to view holograms.</span></span> | <span data-ttu-id="97711-343">ホログラムを表示するには、ユーザーのコンテキストや首部分の一貫性のあるモーションが失われる可能性がありますが必要です。</span><span class="sxs-lookup"><span data-stu-id="97711-343">User likely to lose context and/or consistent neck motion is required to view holograms.</span></span> <span data-ttu-id="97711-344">なし、見つけやすさのガイダンスについては、または縦ホログラム フレームの外側に失われやすくオブジェクトの移動、holographic ラージ オブジェクトのコンテキストのガイダンスには、正規の足部の動きを表示する必要ありません。</span><span class="sxs-lookup"><span data-stu-id="97711-344">No context guidance for large holographic objects, moving objects easy to lose outside the frame with no discoverability guidance, or tall holograms requires regular neck motion to view.</span></span> | 

### <a name="how-to-measure"></a><span data-ttu-id="97711-345">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-345">How to measure</span></span>

* <span data-ttu-id="97711-346">(大) ホログラムのコンテキストが紛失または境界にクリップされているため認識されません。</span><span class="sxs-lookup"><span data-stu-id="97711-346">Context for a (large) hologram is lost or not understood due to being clipped at the boundaries.</span></span>
* <span data-ttu-id="97711-347">ホログラムの場所は、注意取締役や holographic のフレームとの間にすばやく移動できるコンテンツがないのために見つけにくくします。</span><span class="sxs-lookup"><span data-stu-id="97711-347">Location of holograms are hard to find due to the lack of attention directors or content that rapidly moves in and out of the holographic frame.</span></span>
* <span data-ttu-id="97711-348">正規表現での足部の疲労ホログラムを完全に表示するヘッド モーションを上下に反復的なシナリオが必要です。</span><span class="sxs-lookup"><span data-stu-id="97711-348">Scenario requires regular and repetitive up and down head motion to fully see a hologram resulting in neck fatigue.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-349">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-349">Recommendations</span></span>

* <span data-ttu-id="97711-350">視界に合わせて、大きなバージョンを視覚的に移行し、小さなオブジェクトをエクスペリエンスを開始します。</span><span class="sxs-lookup"><span data-stu-id="97711-350">Start the experience with small objects that fit the FOV, then transition with visual cues to larger versions.</span></span>
* <span data-ttu-id="97711-351">空間のオーディオおよび注意ディレクターを使用して、ヘルプ、視界の外にあるユーザーの検索コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="97711-351">Use spatial audio and attention directors to help the user find content that is outside the FOV.</span></span>
* <span data-ttu-id="97711-352">垂直方向にクリップの視界ホログラムが、できる限り多くしないでください。</span><span class="sxs-lookup"><span data-stu-id="97711-352">As much as possible, avoid holograms that vertically clip the FOV.</span></span>
* <span data-ttu-id="97711-353">適切に場所を表示するアプリでのガイダンスをユーザーに提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-353">Provide the user with in-app guidance for best viewing location.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-354">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-354">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-355">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-355">Documentation</span></span>

* [<span data-ttu-id="97711-356">Holographic フレーム</span><span class="sxs-lookup"><span data-stu-id="97711-356">Holographic frame</span></span>](holographic-frame.md)
* [<span data-ttu-id="97711-357">ケース スタディ、HoloStudio UI および相互作用のデザインの学習</span><span class="sxs-lookup"><span data-stu-id="97711-357">Case Study, HoloStudio UI and interaction design learnings</span></span>](case-study-3-holostudio-ui-and-interaction-design-learnings.md?#problem-2-modal-dialogs-are-sometimes-out-of-the-holographic-frame)
* [<span data-ttu-id="97711-358">オブジェクトおよび環境のスケール</span><span class="sxs-lookup"><span data-stu-id="97711-358">Scale of objects and environments</span></span>](scale.md)
* [<span data-ttu-id="97711-359">カーソル、視覚的な合図</span><span class="sxs-lookup"><span data-stu-id="97711-359">Cursors, Visual cues</span></span>](cursors.md#visual-cues)

#### <a name="external-references"></a><span data-ttu-id="97711-360">外部参照</span><span class="sxs-lookup"><span data-stu-id="97711-360">External references</span></span>

* [<span data-ttu-id="97711-361">Ado の利用、FOV</span><span class="sxs-lookup"><span data-stu-id="97711-361">Much ado about the FOV</span></span>](https://www.linkedin.com/pulse/hololens-much-ado-field-of-view-michael-hoffman?lipi=urn%3Ali%3Apage%3Ad_flagship3_feed%3B6iQ%2FbTevLDU93w3I2ewLJw%3D%3D)

## <a name="content-reacts-to-user-position"></a><span data-ttu-id="97711-362">コンテンツがユーザーの位置に対応します。</span><span class="sxs-lookup"><span data-stu-id="97711-362">Content reacts to user position</span></span>

<span data-ttu-id="97711-363">ホログラムは、「実際の」オブジェクトと同じ方法ほぼ内のユーザーの位置に対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-363">Holograms should react to the user position in roughly the same ways that "real" objects do.</span></span> <span data-ttu-id="97711-364">注目すべき設計の考慮事項は、ユーザーの位置を想定できません必ずしも UI 要素が静止していると、ユーザーの動きに合わせては。</span><span class="sxs-lookup"><span data-stu-id="97711-364">A notable design consideration is UI elements that can't necessarily assume a user's position is stationary and adapt to the user's motion.</span></span> <span data-ttu-id="97711-365">ユーザーの位置に正しく対応するアプリをデザインよりかぎりエクスペリエンスの作成し、使いやすきます。</span><span class="sxs-lookup"><span data-stu-id="97711-365">Designing an app that correctly adapts to user position will create a more believable experience and make it easier to use.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-366">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-366">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-367"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-367"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-368"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-368"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-369">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-369">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-370">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-370">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-371">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-371">Quality criteria</span></span>

<table>
<tr>
<td> <span data-ttu-id="97711-372">最高</span><span class="sxs-lookup"><span data-stu-id="97711-372">Best</span></span> </td><td> <span data-ttu-id="97711-373">コンテンツと UI は、自然の想定されるユーザーの移動のスコープ内のコンテンツと対話するユーザーを許可するユーザーの位置に適応します。</span><span class="sxs-lookup"><span data-stu-id="97711-373">Content and UI adapt to user positions allowing user to naturally interact with content within the scope of expected user movement.</span></span></td>
</tr><tr>
<td> <span data-ttu-id="97711-374">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-374">Meets</span></span> </td><td> <span data-ttu-id="97711-375">UI は、ユーザーの位置に対応しますが、それらの位置を調整するユーザーを必要とするキーのコンテンツの表示を妨げる可能性が。</span><span class="sxs-lookup"><span data-stu-id="97711-375">UI adapts to the user position, but may impede the view of key content requiring the user to adjust their position.</span></span></td>
</tr><tr>
<td> <span data-ttu-id="97711-376">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-376">Fail</span></span> </td><td><ol>
<li><span data-ttu-id="97711-377">UI 要素が紛失または、移動の原因となるユーザー コントロールを不自然に戻ります (または見つける) 中にロックされています。</span><span class="sxs-lookup"><span data-stu-id="97711-377">UI elements are lost or locked during movement causing user to unnaturally return to (or find) controls.</span></span></li><li><span data-ttu-id="97711-378">UI 要素は、主要なコンテンツの表示を制限します。</span><span class="sxs-lookup"><span data-stu-id="97711-378">UI elements limit the view of primary content.</span></span></li><li><span data-ttu-id="97711-379">特に、運動量との距離を表示するため UI の動きが最適化されていない<a href="billboarding-and-tag-along.md">tag-along</a> UI 要素。</span><span class="sxs-lookup"><span data-stu-id="97711-379">UI movement is not optimized for viewing distance and momentum particularly with <a href="billboarding-and-tag-along.md">tag-along</a> UI elements.</span></span></li>
</ol></td>
</tr>
</table>

### <a name="how-to-measure"></a><span data-ttu-id="97711-380">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-380">How to measure</span></span>

* <span data-ttu-id="97711-381">すべての測定値は、シナリオの妥当な範囲内で行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-381">All measurements should be done within a reasonable scope of the scenario.</span></span> <span data-ttu-id="97711-382">ユーザーの移動はによって異なりますが、極端なユーザーの移動は、アプリをください。</span><span class="sxs-lookup"><span data-stu-id="97711-382">While user movement will vary, don’t try to trick the app with extreme user movement.</span></span>
* <span data-ttu-id="97711-383">UI 要素、関連するコントロールをユーザーの移動に関係なく利用してください。</span><span class="sxs-lookup"><span data-stu-id="97711-383">For UI elements, relevant controls should be available regardless of user movement.</span></span> <span data-ttu-id="97711-384">たとえば、ユーザーが表示とズームを使用して 3D マップを歩きながら、ズーム コントロールが場所に関係なく、ユーザーにすぐに使用できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-384">For example, if the user is viewing and walking around a 3D map with zoom, the zoom control should be readily available to the user regardless of location.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-385">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-385">Recommendations</span></span>

* <span data-ttu-id="97711-386">ユーザーは、カメラであり、動作を制御します。</span><span class="sxs-lookup"><span data-stu-id="97711-386">The user is the camera and they control the movement.</span></span> <span data-ttu-id="97711-387">ドライブにできるようにします。</span><span class="sxs-lookup"><span data-stu-id="97711-387">Let them drive.</span></span>
* <span data-ttu-id="97711-388">テキストのためのビルボードを検討してくださいされ帰りシステム world ロックや非表示になる場合、ユーザー、それ以外の場合に移動します。</span><span class="sxs-lookup"><span data-stu-id="97711-388">Consider billboarding for text and menuing systems that would otherwise be world-locked or obscured if a user were to move around.</span></span>
* <span data-ttu-id="97711-389">前に新機能については、ユーザーを許可する一方、ユーザーをフォローする必要があるコンテンツの tag-along を使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-389">Use tag-along for content that needs to follow the user while still allowing the user to see what is in front of them.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-390">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-390">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-391">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-391">Documentation</span></span>

* [<span data-ttu-id="97711-392">対話デザイン</span><span class="sxs-lookup"><span data-stu-id="97711-392">Interaction design</span></span>](hologram.md)
* [<span data-ttu-id="97711-393">色、光、および資料</span><span class="sxs-lookup"><span data-stu-id="97711-393">Color, light, and material</span></span>](color,-light-and-materials.md)
* [<span data-ttu-id="97711-394">ビルボード処理と tag-along</span><span class="sxs-lookup"><span data-stu-id="97711-394">Billboarding and tag-along</span></span>](billboarding-and-tag-along.md)
* [<span data-ttu-id="97711-395">相互作用の基礎</span><span class="sxs-lookup"><span data-stu-id="97711-395">Interaction fundamentals</span></span>](interaction-fundamentals.md)
* [<span data-ttu-id="97711-396">自己モーションとユーザー locomotion</span><span class="sxs-lookup"><span data-stu-id="97711-396">Self-motion and user locomotion</span></span>](comfort.md#self-motion-and-user-locomotion)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-397">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-397">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-398">MR 入力 210:視線入力</span><span class="sxs-lookup"><span data-stu-id="97711-398">MR Input 210: Gaze</span></span>](holograms-210.md)

## <a name="input-interaction-clarity"></a><span data-ttu-id="97711-399">入力の相互作用をわかりやすくするため</span><span class="sxs-lookup"><span data-stu-id="97711-399">Input interaction clarity</span></span>

<span data-ttu-id="97711-400">入力の相互作用をわかりやすくするためは、アプリの有用性に重大な入力の整合性、未成熟、見つけやすさの相互作用の方法が含まれています。</span><span class="sxs-lookup"><span data-stu-id="97711-400">Input interaction clarity is critical to an app's usability and includes input consistency, approachability, discoverability of interaction methods.</span></span> <span data-ttu-id="97711-401">ユーザーは、再確認せずにプラットフォーム全体にわたる一般的な相互作用を使用できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-401">User should be able to use platform-wide common interactions without relearning.</span></span> <span data-ttu-id="97711-402">アプリにカスタムの入力がある場合が明確に伝達し、説明する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-402">If the app has custom input, it should be clearly communicated and demonstrated.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-403">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-403">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-404"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-404"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-405"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-405"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-406">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-406">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-407">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-407">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-408">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-408">Quality criteria</span></span>

|  <span data-ttu-id="97711-409">最高</span><span class="sxs-lookup"><span data-stu-id="97711-409">Best</span></span>  |  <span data-ttu-id="97711-410">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-410">Meets</span></span> |  <span data-ttu-id="97711-411">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-411">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-412">入力の対話操作のメソッドは提供されている Windows Mixed Reality で一貫性のある[ガイダンス](interaction-fundamentals.md)します。</span><span class="sxs-lookup"><span data-stu-id="97711-412">Input interaction methods are consistent with Windows Mixed Reality provided [guidance](interaction-fundamentals.md).</span></span> <span data-ttu-id="97711-413">任意のカスタム入力標準入力 (使用して標準的な対話ではなく) と重複することはできません必要があります明確に伝達およびユーザーに示されています。</span><span class="sxs-lookup"><span data-stu-id="97711-413">Any custom input should not be redundant with standard input (rather use standard interaction) and must be clearly communicated and demonstrated to the user.</span></span> | <span data-ttu-id="97711-414">同様に最適ですがカスタムの入力は、標準入力方式を冗長です。</span><span class="sxs-lookup"><span data-stu-id="97711-414">Similar to best, but custom inputs are redundant with standard input methods.</span></span> <span data-ttu-id="97711-415">ユーザーの目標とアプリ エクスペリエンスの進行状況を実現できます。</span><span class="sxs-lookup"><span data-stu-id="97711-415">User can still achieve the goal and progress through the app experience.</span></span> | <span data-ttu-id="97711-416">入力メソッドまたはボタンのマッピングを理解するのには困難です。</span><span class="sxs-lookup"><span data-stu-id="97711-416">Difficult to understand input method or button mapping.</span></span> <span data-ttu-id="97711-417">入力が大きくカスタマイズされて、なしの手順については、標準の入力をサポートしていませんまたは疲労と快適性の問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="97711-417">Input is heavily customized, does not support standard input, no instructions, or likely to cause fatigue and comfort issues.</span></span> | 

### <a name="how-to-measure"></a><span data-ttu-id="97711-418">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-418">How to measure</span></span>

* <span data-ttu-id="97711-419">アプリで使用する一貫性のある[標準入力方式。](interaction-fundamentals.md)</span><span class="sxs-lookup"><span data-stu-id="97711-419">The app uses consistent [standard input methods.](interaction-fundamentals.md)</span></span>
* <span data-ttu-id="97711-420">アプリにカスタムの入力がある場合は、それを明確にを通じてを伝達します。</span><span class="sxs-lookup"><span data-stu-id="97711-420">If the app has custome input, it is clearly communicated through:</span></span>
* <span data-ttu-id="97711-421">最初の実行エクスペリエンス</span><span class="sxs-lookup"><span data-stu-id="97711-421">First-run experience</span></span>
* <span data-ttu-id="97711-422">概要画面</span><span class="sxs-lookup"><span data-stu-id="97711-422">Introductory screens</span></span>
* <span data-ttu-id="97711-423">ヒント</span><span class="sxs-lookup"><span data-stu-id="97711-423">Tooltips</span></span>
* <span data-ttu-id="97711-424">手動指導者</span><span class="sxs-lookup"><span data-stu-id="97711-424">Hand coach</span></span>
* <span data-ttu-id="97711-425">ヘルプ セクション</span><span class="sxs-lookup"><span data-stu-id="97711-425">Help section</span></span>
* <span data-ttu-id="97711-426">ボイス オーバー</span><span class="sxs-lookup"><span data-stu-id="97711-426">Voice over</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-427">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-427">Recommendations</span></span>

* <span data-ttu-id="97711-428">可能な限り標準の入力メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-428">Use standard input methods whenever possible.</span></span>
* <span data-ttu-id="97711-429">標準以外の入力方法のデモ、チュートリアル、およびツールヒントを提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-429">Provide demonstrations, tutorials, and tooltips for non-standard input methods.</span></span>
* <span data-ttu-id="97711-430">アプリ全体で一貫性のある相互作用モデルを使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-430">Use a consistent interaction model throughout the app.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-431">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-431">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-432">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-432">Documentation</span></span>

* [<span data-ttu-id="97711-433">Windows MR 相互作用の基礎</span><span class="sxs-lookup"><span data-stu-id="97711-433">Windows MR interaction fundamentals</span></span>](interaction-fundamentals.md)
* [<span data-ttu-id="97711-434">対話型のオブジェクト</span><span class="sxs-lookup"><span data-stu-id="97711-434">Interactable objects</span></span>](interactable-object.md)
* [<span data-ttu-id="97711-435">視線の先を対象とします。</span><span class="sxs-lookup"><span data-stu-id="97711-435">Gaze targeting</span></span>](gaze-targeting.md)
* [<span data-ttu-id="97711-436">カーソル</span><span class="sxs-lookup"><span data-stu-id="97711-436">Cursors</span></span>](cursors.md)
* [<span data-ttu-id="97711-437">快適性と視線入力</span><span class="sxs-lookup"><span data-stu-id="97711-437">Comfort and gaze</span></span>](comfort.md#gaze-direction)
* [<span data-ttu-id="97711-438">ジェスチャ</span><span class="sxs-lookup"><span data-stu-id="97711-438">Gestures</span></span>](gestures.md)
* [<span data-ttu-id="97711-439">音声入力</span><span class="sxs-lookup"><span data-stu-id="97711-439">Voice input</span></span>](voice-input.md)
* [<span data-ttu-id="97711-440">音声のデザイン</span><span class="sxs-lookup"><span data-stu-id="97711-440">Voice design</span></span>](voice-design.md)
* [<span data-ttu-id="97711-441">アニメーション コント ローラー</span><span class="sxs-lookup"><span data-stu-id="97711-441">Motion controllers</span></span>](motion-controllers.md)
* [<span data-ttu-id="97711-442">Unity のガイドの移植の入力</span><span class="sxs-lookup"><span data-stu-id="97711-442">Input porting guide for Unity</span></span>](input-porting-guide-for-unity.md)
* [<span data-ttu-id="97711-443">Unity におけるキーボード入力</span><span class="sxs-lookup"><span data-stu-id="97711-443">Keyboard input in Unity</span></span>](keyboard-input-in-unity.md)
* [<span data-ttu-id="97711-444">これで Unity</span><span class="sxs-lookup"><span data-stu-id="97711-444">Gaze in Unity</span></span>](gaze-in-unity.md)
* [<span data-ttu-id="97711-445">ジェスチャと Unity のアニメーション コント ローラー</span><span class="sxs-lookup"><span data-stu-id="97711-445">Gestures and motion controllers in Unity</span></span>](gestures-and-motion-controllers-in-unity.md)
* [<span data-ttu-id="97711-446">Unity での音声入力</span><span class="sxs-lookup"><span data-stu-id="97711-446">Voice input in Unity</span></span>](voice-input-in-unity.md)
* [<span data-ttu-id="97711-447">キーボード、マウス、および DirectX でコント ローラーの入力</span><span class="sxs-lookup"><span data-stu-id="97711-447">Keyboard, mouse, and controller input in DirectX</span></span>](keyboard,-mouse,-and-controller-input-in-directx.md)
* [<span data-ttu-id="97711-448">視線、ジェスチャ、および DirectX でモーション コント ローラー</span><span class="sxs-lookup"><span data-stu-id="97711-448">Gaze, gesture, and motion controllers in DirectX</span></span>](gaze,-gestures,-and-motion-controllers-in-directx.md)
* [<span data-ttu-id="97711-449">DirectX での音声入力</span><span class="sxs-lookup"><span data-stu-id="97711-449">Voice input in DirectX</span></span>](voice-input-in-directx.md)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-450">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-450">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-451">ケース スタディ:複数のパーソナル コンピューティングのフォロー アップ</span><span class="sxs-lookup"><span data-stu-id="97711-451">Case study: The pursuit of more personal computing</span></span>](case-study-the-pursuit-of-more-personal-computing.md#less-interface-in-your-face)
* [<span data-ttu-id="97711-452">調査をキャストします。HoloStudio UI との対話デザインの学習内容</span><span class="sxs-lookup"><span data-stu-id="97711-452">Cast study: HoloStudio UI and interaction design learnings</span></span>](case-study-3-holostudio-ui-and-interaction-design-learnings.md)
* [<span data-ttu-id="97711-453">サンプル アプリ:要素の定期処理テーブル</span><span class="sxs-lookup"><span data-stu-id="97711-453">Sample app: Periodic table of the elements</span></span>](periodic-table-of-the-elements.md)
* [<span data-ttu-id="97711-454">サンプル アプリ:旧暦モジュール</span><span class="sxs-lookup"><span data-stu-id="97711-454">Sample app: Lunar module</span></span>](lunar-module.md)
* [<span data-ttu-id="97711-455">MR 入力 210:視線入力</span><span class="sxs-lookup"><span data-stu-id="97711-455">MR Input 210: Gaze</span></span>](holograms-210.md)
* [<span data-ttu-id="97711-456">MR 入力 211:ジェスチャ</span><span class="sxs-lookup"><span data-stu-id="97711-456">MR Input 211: Gestures</span></span>](holograms-211.md)
* [<span data-ttu-id="97711-457">MR 入力 212:音声</span><span class="sxs-lookup"><span data-stu-id="97711-457">MR Input 212: Voice</span></span>](holograms-212.md)

## <a name="interactable-objects"></a><span data-ttu-id="97711-458">対話型のオブジェクト</span><span class="sxs-lookup"><span data-stu-id="97711-458">Interactable objects</span></span>

<span data-ttu-id="97711-459">ボタンには、2 D 抽象世界でイベントをトリガーに使用されるメタファが長年です。</span><span class="sxs-lookup"><span data-stu-id="97711-459">A button has long been a metaphor used for triggering an event in the 2D abstract world.</span></span> <span data-ttu-id="97711-460">3 次元の複合現実の世界では、この抽象化はもはやの世界に限定しました必要はありません。</span><span class="sxs-lookup"><span data-stu-id="97711-460">In the three-dimensional mixed reality world, we don’t have to be confined to this world of abstraction anymore.</span></span> <span data-ttu-id="97711-461">イベントをトリガーする対話型のオブジェクトを何も指定できます。</span><span class="sxs-lookup"><span data-stu-id="97711-461">Anything can be an Interactable object that triggers an event.</span></span> <span data-ttu-id="97711-462">対話型のオブジェクトは、そのテーブルに、コーヒー カップから空中に浮かんでバルーンをものとして表現できます。</span><span class="sxs-lookup"><span data-stu-id="97711-462">An interactable object can be represented as anything from a coffee cup on the table to a balloon floating in the air.</span></span> <span data-ttu-id="97711-463">形式に関係なく対話型のオブジェクトを視覚的およびオーディオをユーザーが明確に認識できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-463">Regardless of the form, interactable objects should be clearly recognizable by the user through visual and audio cues.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-464">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-464">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-465"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-465"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-466"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-466"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-467">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-467">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-468">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-468">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-469">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-469">Quality criteria</span></span>

|  <span data-ttu-id="97711-470">最高</span><span class="sxs-lookup"><span data-stu-id="97711-470">Best</span></span>  |  <span data-ttu-id="97711-471">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-471">Meets</span></span> |  <span data-ttu-id="97711-472">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-472">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-473">3 つの状態の間で視覚的およびオーディオを認識できるものは対話型のオブジェクト、形式に関係なく: アイドル状態をターゲットとして、選択します。</span><span class="sxs-lookup"><span data-stu-id="97711-473">Regardless of form, interactable objects are recognizable through visual and audio cues across three states: idle, targeted, and selected.</span></span> <span data-ttu-id="97711-474">「に言ってを参照してください」がオフで、一貫した使用エクスペリエンスのあらゆる場所。</span><span class="sxs-lookup"><span data-stu-id="97711-474">"See it, say it" is clear and consistently used throughout the experience.</span></span> <span data-ttu-id="97711-475">オブジェクトは拡大縮小され、エラーを対象とする無料のために分散します。</span><span class="sxs-lookup"><span data-stu-id="97711-475">Objects are scaled and distributed to allow for error free targeting.</span></span> | <span data-ttu-id="97711-476">ユーザーできますオーディオまたはビデオのフィードバックを通じた対話型としてオブジェクトを認識およびできますターゲットし、オブジェクトをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="97711-476">User can recognize object as interactable through audio or visual feedback, and can target and activate the object.</span></span> | <span data-ttu-id="97711-477">ビジュアルやオーディオ キューを指定しない場合は、ユーザーは対話型のオブジェクトを認識できません。</span><span class="sxs-lookup"><span data-stu-id="97711-477">Given no visual or audio cues, user cannot recognize an interactable object.</span></span> <span data-ttu-id="97711-478">相互作用は、間違いやすくオブジェクト スケールまたはオブジェクト間の距離が原因です。</span><span class="sxs-lookup"><span data-stu-id="97711-478">Interactions are error prone due to object scale or distance between objects.</span></span> | 

### <a name="how-to-measure"></a><span data-ttu-id="97711-479">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-479">How to measure</span></span>

* <span data-ttu-id="97711-480">対話型のオブジェクトが '対話型'; として認識できます。特定のボタン、メニューのおよびアプリのコンテンツを含むです。</span><span class="sxs-lookup"><span data-stu-id="97711-480">Interactable objects are recognizable as 'interactable'; including buttons, menus, and app specific content.</span></span> <span data-ttu-id="97711-481">経験則として必要がありますビジュアルおよびオーディオ キュー対話型のオブジェクトを対象とする場合。</span><span class="sxs-lookup"><span data-stu-id="97711-481">As a rule of thumb there should be a visual and audio cue when targeting interactable objects.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-482">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-482">Recommendations</span></span>

* <span data-ttu-id="97711-483">相互作用のビジュアルおよびオーディオのフィードバックを使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-483">Use visual and audio feedback for interactions.</span></span>
* <span data-ttu-id="97711-484">それぞれの入力 (アイドル状態、対象となる、選択した) の状態の視覚的なフィードバックを区別する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-484">Visual feedback should be differentiated for each input state (idle, targeted, selected)</span></span>
* <span data-ttu-id="97711-485">対話型のオブジェクトを拡張し、エラーを対象とする無料の配置する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-485">Interactable objects should be scaled and placed for error free targeting.</span></span>
* <span data-ttu-id="97711-486">(メニュー バーやリスト) グループ化された対話型のオブジェクトには、適切な間隔を対象とする必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-486">Grouped interactable objects (such as a menu bar or list) should have proper spacing for targeting.</span></span>
* <span data-ttu-id="97711-487">音声コマンドをサポートするボタンとメニューは、キーワードのコマンドのテキスト ラベルを指定する必要があります (「表示, に言って」)</span><span class="sxs-lookup"><span data-stu-id="97711-487">Buttons and menus that support voice command should provide text labels for the command keyword ("See it, say it")</span></span>

### <a name="resources"></a><span data-ttu-id="97711-488">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-488">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-489">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-489">Documentation</span></span>

* [<span data-ttu-id="97711-490">対話型のオブジェクト</span><span class="sxs-lookup"><span data-stu-id="97711-490">Interactable object</span></span>](interactable-object.md)
* [<span data-ttu-id="97711-491">Unity 内のテキスト</span><span class="sxs-lookup"><span data-stu-id="97711-491">Text in Unity</span></span>](text-in-unity.md)
* [<span data-ttu-id="97711-492">アプリ バー、境界ボックス</span><span class="sxs-lookup"><span data-stu-id="97711-492">App bar and bounding box</span></span>](app-bar-and-bounding-box.md)
* [<span data-ttu-id="97711-493">音声のデザイン</span><span class="sxs-lookup"><span data-stu-id="97711-493">Voice design</span></span>](voice-design.md)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-494">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-494">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-495">Mixed Reality Toolkit - UX</span><span class="sxs-lookup"><span data-stu-id="97711-495">Mixed Reality Toolkit - UX</span></span>](https://github.com/Microsoft/MixedRealityToolkit-Unity/tree/htk_release/Assets/HoloToolkit-Examples/UX)

## <a name="room-scanning"></a><span data-ttu-id="97711-496">ルームのスキャン</span><span class="sxs-lookup"><span data-stu-id="97711-496">Room scanning</span></span>

<span data-ttu-id="97711-497">空間マッピング データを必要とするアプリでは、時間の経過と共に自動的にこのデータを収集するデバイスに依存しており、ユーザーとセッション間でアクティブなデバイスでの環境について説明します。</span><span class="sxs-lookup"><span data-stu-id="97711-497">Apps that require spatial mapping data rely on the device to automatically collect this data over time and across sessions as the user explores their environment with the device active.</span></span> <span data-ttu-id="97711-498">完全を期すため、このデータの品質は、さまざまなユーザーが行った探索の量、探索からどれ時間だけが経過や、デバイス、領域をスキャンするので家具や扉などのオブジェクトが移動するかどうかなどの要因に依存します。</span><span class="sxs-lookup"><span data-stu-id="97711-498">The completeness and quality of this data depends on a number of factors including the amount of exploration the user has done, how much time has passed since the exploration and whether objects such as furniture and doors have moved since the device scanned the area.</span></span> <span data-ttu-id="97711-499">多くのアプリでは、ユーザーが、完全を期すためと、空間のマップの品質を向上させるために追加の手順を実行する必要があるかどうかを判断するエクスペリエンスの先頭に空間マッピング データを分析します。</span><span class="sxs-lookup"><span data-stu-id="97711-499">Many apps will analyze the spatial mapping data at the start of the experience to judge whether the user should perform additional steps to improve the completeness and quality of the spatial map.</span></span> <span data-ttu-id="97711-500">場合は、ユーザーが、スキャン時にガイダンスが提供される必要があります明確、環境をスキャンするために必要です。</span><span class="sxs-lookup"><span data-stu-id="97711-500">If the user is required to scan the environment, clear guidance should be provided during the scanning experience.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-501">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-501">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-502"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-502"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-503"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-503"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-504">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-504">✔️</span></span></td><td style="text-align: center;"></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-505">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-505">Quality criteria</span></span>

|  <span data-ttu-id="97711-506">最高</span><span class="sxs-lookup"><span data-stu-id="97711-506">Best</span></span>  |  <span data-ttu-id="97711-507">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-507">Meets</span></span> |  <span data-ttu-id="97711-508">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-508">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-509">空間メッシュの視覚化は、ユーザーのスキャンが進行中に伝えます。</span><span class="sxs-lookup"><span data-stu-id="97711-509">Visualization of the spatial mesh tell users scanning is in progress.</span></span> <span data-ttu-id="97711-510">ユーザーは、対処方法と、スキャンが開始し、停止に明確に認識しています。</span><span class="sxs-lookup"><span data-stu-id="97711-510">User clearly knows what to do and when the scan starts and stops.</span></span> | <span data-ttu-id="97711-511">空間のメッシュの視覚エフェクトが提供されますが、ユーザーが明確に対処できないを行うと進行状況に関する情報は提供されません。</span><span class="sxs-lookup"><span data-stu-id="97711-511">Visualization of the spatial mesh is provided, but the user may not clearly know what to do and no progress information is provided.</span></span> | <span data-ttu-id="97711-512">メッシュの視覚表現はありません。</span><span class="sxs-lookup"><span data-stu-id="97711-512">No visualization of mesh.</span></span> <span data-ttu-id="97711-513">ガイダンスの情報を探すには、where 句またはときに、スキャンを開始または停止についてユーザーに提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-513">No guidance information provided to the user regarding where to look, or when the scan starts/stops.</span></span> |

### <a name="how-to-measure"></a><span data-ttu-id="97711-514">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-514">How to measure</span></span>

* <span data-ttu-id="97711-515">必要なルーム スキャン中に、検索する場所を開始して停止のスキャンを示すビジュアルおよびオーディオのガイダンスが提供されます。</span><span class="sxs-lookup"><span data-stu-id="97711-515">During a required room scan, visual and audio guidance is provided indicating where to look, and when to start and stop scanning.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-516">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-516">Recommendations</span></span>

* <span data-ttu-id="97711-517">エクスペリエンスの一部である必要があるユーザーの近くの合計ボリュームの量を指定します。</span><span class="sxs-lookup"><span data-stu-id="97711-517">Indicate how much of the total volume in the users vicinity needs to be part of the experience.</span></span>
* <span data-ttu-id="97711-518">スキャンが開始され、進行状況インジケーターなどを停止すると通信します。</span><span class="sxs-lookup"><span data-stu-id="97711-518">Communicate when the scan starts and stops such as a progress indicator.</span></span>
* <span data-ttu-id="97711-519">スキャン中に、メッシュの視覚エフェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-519">Use a visualization of the mesh during the scan.</span></span>
* <span data-ttu-id="97711-520">検索し、ルーム内を移動するユーザーを促すビジュアルおよびオーディオの手掛かりを提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-520">Provide visual and audio cues to encourage the user to look and move around the room.</span></span>
* <span data-ttu-id="97711-521">データを向上させるために移動する場所をユーザーに通知します。</span><span class="sxs-lookup"><span data-stu-id="97711-521">Inform the user where to go to improve the data.</span></span> <span data-ttu-id="97711-522">多くの場合に必要な内容の操作を行います (例: を見て、ceiling 見て家具の背後にある)、ユーザーに伝えるための最適な場合があります、スキャンのために必要な品質を取得するためにします。</span><span class="sxs-lookup"><span data-stu-id="97711-522">In many cases, it may be best to tell the user what they need to do (e.g. look at the ceiling, look behind furniture), in order to get the necessary scan quality.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-523">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-523">Resources</span></span>

#### <a name="documentation"></a><span data-ttu-id="97711-524">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="97711-524">Documentation</span></span>

* [<span data-ttu-id="97711-525">ルームのスキャンの視覚化</span><span class="sxs-lookup"><span data-stu-id="97711-525">Room scan visualization</span></span>](room-scan-visualization.md)
* [<span data-ttu-id="97711-526">ケース スタディ:HoloLens の空間のマッピング機能を展開します。</span><span class="sxs-lookup"><span data-stu-id="97711-526">Case study: Expanding the spatial mapping capabilities of HoloLens</span></span>](case-study-expanding-the-spatial-mapping-capabilities-of-hololens.md)
* [<span data-ttu-id="97711-527">ケース スタディ:空間 HoloTour の設計</span><span class="sxs-lookup"><span data-stu-id="97711-527">Case study: Spatial sound design for HoloTour</span></span>](case-study-spatial-sound-design-for-holotour.md)
* [<span data-ttu-id="97711-528">ケース スタディ:フラグメントで魅力的なエクスペリエンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="97711-528">Case study: Creating an immersive experience in Fragments</span></span>](case-study-creating-an-immersive-experience-in-fragments.md)

#### <a name="tools-and-tutorials"></a><span data-ttu-id="97711-529">ツールとチュートリアル</span><span class="sxs-lookup"><span data-stu-id="97711-529">Tools and tutorials</span></span>

* [<span data-ttu-id="97711-530">Mixed Reality Toolkit - UX</span><span class="sxs-lookup"><span data-stu-id="97711-530">Mixed Reality Toolkit - UX</span></span>](https://github.com/Microsoft/MixedRealityToolkit-Unity/tree/htk_release/Assets/HoloToolkit-Examples/UX)

## <a name="directional-indicators"></a><span data-ttu-id="97711-531">方向インジケーター</span><span class="sxs-lookup"><span data-stu-id="97711-531">Directional indicators</span></span>

<span data-ttu-id="97711-532">Mixed reality アプリでは、コンテンツは、ビューのフィールドの外側にありますか、現実世界のオブジェクトによってオクルー ジョンします。</span><span class="sxs-lookup"><span data-stu-id="97711-532">In a mixed reality app, content may be outside the field of view or occluded by real-world objects.</span></span> <span data-ttu-id="97711-533">適切に設計されたアプリは簡単に表示されているコンテンツを検索するユーザー。</span><span class="sxs-lookup"><span data-stu-id="97711-533">A well designed app will make it easier for the user to find non-visible content.</span></span> <span data-ttu-id="97711-534">方向インジケーターは、重要なコンテンツをユーザーに警告し、ユーザーの位置を基準としたコンテンツへのガイダンスを提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-534">Directional indicators alert a user to important content and provide guidance to the content relative to the user's position.</span></span> <span data-ttu-id="97711-535">非表示のコンテンツへのガイダンスには、サウンドのエミッタ、方向矢印、または直接の視覚的な手掛かりのフォームを実行できます。</span><span class="sxs-lookup"><span data-stu-id="97711-535">Guidance to non-visible content can take the form of sound emitters, directional arrows, or direct visual cues.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-536">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-536">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-537"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-537"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-538"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-538"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-539">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-539">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-540">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-540">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-541">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-541">Quality criteria</span></span>

|  <span data-ttu-id="97711-542">最高</span><span class="sxs-lookup"><span data-stu-id="97711-542">Best</span></span>  |  <span data-ttu-id="97711-543">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-543">Meets</span></span> |  <span data-ttu-id="97711-544">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-544">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-545">ビジュアルおよびオーディオ キューは、ビューのフィールドの外側の関連するコンテンツに直接ユーザーを説明します。</span><span class="sxs-lookup"><span data-stu-id="97711-545">Visual and audio cues directly guide the user to relevant content outside the field of view.</span></span> | <span data-ttu-id="97711-546">矢印またはコンテンツの全体的な方向性で、ユーザーを示すいくつかのインジケーター。</span><span class="sxs-lookup"><span data-stu-id="97711-546">An arrow or some indicator that points the user in the general direction of the content.</span></span> | <span data-ttu-id="97711-547">関連するコンテンツが視野、外部と低いか、ユーザーに場所のガイダンスは提供されません。</span><span class="sxs-lookup"><span data-stu-id="97711-547">Relevant content is outside of the field of view, and poor or no location guidance is provided to the user.</span></span> | 

### <a name="how-to-measure"></a><span data-ttu-id="97711-548">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-548">How to measure</span></span>

* <span data-ttu-id="97711-549">ビューのユーザー フィールドの外部で関連するコンテンツでは、ビジュアルおよびオーディオ キューを検出します。</span><span class="sxs-lookup"><span data-stu-id="97711-549">Relevant content outside of the user field of view is discoverable through visual and/or audio cues.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-550">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-550">Recommendations</span></span>

* <span data-ttu-id="97711-551">関連するコンテンツは、外部のユーザーのフィールドの表示が、コンテンツにユーザーをガイドするのに方向インジケーターとオーディオ キューを使用します。</span><span class="sxs-lookup"><span data-stu-id="97711-551">When relevant content is outside the user's field of view, use directional indicators and audio cues to guide the user to the content.</span></span> <span data-ttu-id="97711-552">多くの場合、直接 visual ガイドことをお勧め方向矢印にします。</span><span class="sxs-lookup"><span data-stu-id="97711-552">In many cases, a direct visual guide is preferred over directional arrows.</span></span>
* <span data-ttu-id="97711-553">方向インジケーターは、カーソルに組み込まないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="97711-553">Directional indicators should not be built into the cursor.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-554">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-554">Resources</span></span>

* [<span data-ttu-id="97711-555">Holographic フレーム</span><span class="sxs-lookup"><span data-stu-id="97711-555">Holographic frame</span></span>](holographic-frame.md)

## <a name="data-loading"></a><span data-ttu-id="97711-556">データの読み込み</span><span class="sxs-lookup"><span data-stu-id="97711-556">Data loading</span></span>

<span data-ttu-id="97711-557">プログレス コントロールは、時間のかかる操作が進行中であることを示すフィードバックをユーザーに返します。</span><span class="sxs-lookup"><span data-stu-id="97711-557">A progress control provides feedback to the user that a long-running operation is underway.</span></span> <span data-ttu-id="97711-558">ユーザーは、進行状況インジケーターが表示されると、待機時間はどれくらいの時間ありますを示すことも、アプリで操作できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="97711-558">It can mean that the user cannot interact with the app when the progress indicator is visible and can also indicate how long the wait time might be.</span></span>

### <a name="device-impact"></a><span data-ttu-id="97711-559">デバイスへの影響</span><span class="sxs-lookup"><span data-stu-id="97711-559">Device impact</span></span>

<table>
<tr>
<th style="width:150px"> <span data-ttu-id="97711-560"><a href="hololens-hardware-details.md">HoloLens</a></span><span class="sxs-lookup"><span data-stu-id="97711-560"><a href="hololens-hardware-details.md">HoloLens</a></span></span></th><th style="width:150px"> <span data-ttu-id="97711-561"><a href="immersive-headset-hardware-details.md">イマーシブ ヘッドセット</a></span><span class="sxs-lookup"><span data-stu-id="97711-561"><a href="immersive-headset-hardware-details.md">Immersive headsets</a></span></span></th>
</tr><tr>
<td style="text-align: center;"> <span data-ttu-id="97711-562">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-562">✔️</span></span></td><td style="text-align: center;"> <span data-ttu-id="97711-563">✔️</span><span class="sxs-lookup"><span data-stu-id="97711-563">✔️</span></span></td>
</tr>
</table>

### <a name="quality-criteria"></a><span data-ttu-id="97711-564">品質基準</span><span class="sxs-lookup"><span data-stu-id="97711-564">Quality criteria</span></span>

|  <span data-ttu-id="97711-565">最高</span><span class="sxs-lookup"><span data-stu-id="97711-565">Best</span></span>  |  <span data-ttu-id="97711-566">満たす</span><span class="sxs-lookup"><span data-stu-id="97711-566">Meets</span></span> |  <span data-ttu-id="97711-567">失敗</span><span class="sxs-lookup"><span data-stu-id="97711-567">Fail</span></span> |
--- | --- | ---
|  <span data-ttu-id="97711-568">進行状況バーや任意のデータの読み込みまたは処理中に進行状況を示すリングの形式で、視覚的なインジケーターをアニメーション化します。</span><span class="sxs-lookup"><span data-stu-id="97711-568">Animated visual indicator, in the form of a progress bar or ring, showing progress during any data loading or processing.</span></span> <span data-ttu-id="97711-569">視覚インジケータは、どのくらいの時間待機する可能性がありますにガイダンスを提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-569">The visual indicator provides guidance on how long the wait could be.</span></span> | <span data-ttu-id="97711-570">データの読み込みが進行中ではどのくらいの時間、待機できることを示す値はありませんが、ユーザーが通知されます。</span><span class="sxs-lookup"><span data-stu-id="97711-570">User is informed that data loading is in progress, but there is no indication of how long the wait could be.</span></span> | <span data-ttu-id="97711-571">データの読み込みまたはプロセスのインジケーターを 5 秒以上かかったタスクがありません。</span><span class="sxs-lookup"><span data-stu-id="97711-571">No data loading or process indicators for task taking longer than 5 seconds.</span></span> |

### <a name="how-to-measure"></a><span data-ttu-id="97711-572">測定する方法</span><span class="sxs-lookup"><span data-stu-id="97711-572">How to measure</span></span>

* <span data-ttu-id="97711-573">データの読み込み中には、5 秒以上の空の状態はありませんを確認します。</span><span class="sxs-lookup"><span data-stu-id="97711-573">During data loading verify there is no blank state for more than 5 seconds.</span></span>

### <a name="recommendations"></a><span data-ttu-id="97711-574">推奨事項</span><span class="sxs-lookup"><span data-stu-id="97711-574">Recommendations</span></span>

* <span data-ttu-id="97711-575">ユーザーがこのアプリが停止しているか、クラッシュするを感じる可能性がある場合に、どのような状況で進行状況を示すデータ読み込み animator を提供します。</span><span class="sxs-lookup"><span data-stu-id="97711-575">Provide a data loading animator showing progress in any situation when the user may perceive this app to have stalled or crashed.</span></span> <span data-ttu-id="97711-576">妥当な経験則は、'ロード' アクティビティで 5 秒以上かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="97711-576">A reasonable rule of thumb is any 'loading' activity that could take more than 5 seconds.</span></span>

### <a name="resources"></a><span data-ttu-id="97711-577">参考資料</span><span class="sxs-lookup"><span data-stu-id="97711-577">Resources</span></span>

* [<span data-ttu-id="97711-578">進行状況の表示</span><span class="sxs-lookup"><span data-stu-id="97711-578">Displaying progress</span></span>](progress.md)