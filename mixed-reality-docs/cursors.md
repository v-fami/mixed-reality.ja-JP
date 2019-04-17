---
title: カーソル
description: カーソル、または、ターゲットのベクターのインジケーターは、各自の意志について理解して HoloLens を理解するユーザーの継続的なフィードバックを提供します。
author: thetuvix
ms.author: alexturn, thgable
ms.date: 02/24/2019
ms.topic: article
keywords: HoloLens (第 1 世代) HoloLens 2、Mixed Reality、カーソル、対象とする、視線、ジェスチャ
ms.openlocfilehash: cdedcaffabe0f90e7956fdb19a7b85e202fcf403
ms.sourcegitcommit: 384b0087899cd835a3a965f75c6f6c607c9edd1b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/12/2019
ms.locfileid: "59604658"
---
# <a name="cursors"></a><span data-ttu-id="5dba5-104">カーソル</span><span class="sxs-lookup"><span data-stu-id="5dba5-104">Cursors</span></span>

> [!NOTE]
> <span data-ttu-id="5dba5-105">HoloLens 2 に固有のガイダンスについて[近日](index.md#news-and-notes)します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-105">More guidance specific to HoloLens 2 [coming soon](index.md#news-and-notes).</span></span>


<span data-ttu-id="5dba5-106">カーソル、または、現在対象とするベクトルのインジケーターは、HoloLens が、現在のフォーカスを認識する場所を理解するユーザーの継続的なフィードバックは、その時点で提供します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-106">A cursor, or indicator of your current targeting vector, provides continuous feedback for the user to understand where HoloLens believes their current focus is at that time.</span></span> <span data-ttu-id="5dba5-107">カーソルは、現在のターゲットを理解するユーザーをポイントし、入力に応答をどのような領域、ホログラム、またはポイントを示すためにフィードバックとして機能できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-107">The cursor allows the user to understand their current targeting point and acts as feedback to indicate what area, hologram, or point will respond to input.</span></span> <span data-ttu-id="5dba5-108">デジタル形式のデバイスが (各自の意志について何かを決定すると同じが存在する可能性がありますしない) 場合に、ユーザーの注意を理解します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-108">It is the digital representation of where the device understands the user's attention to be (though that may not be the same as determining anything about their intentions).</span></span>

<span data-ttu-id="5dba5-109">カーソルによって提供されるフィードバックは、システムの応答方法を予測する機能をユーザーに提供をデバイスに、目的のコミュニケーションを改善しが最終的には、安心してそれらの相互作用に関するフィードバックとしてそのシグナルを使用します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-109">The feedback provided by the cursor offers users the ability to anticipate how the system will respond, use that signal as feedback to better communicate their intention to the device, and ultimately be more confident about their interactions.</span></span>

## <a name="hololens-1st-gen"></a><span data-ttu-id="5dba5-110">HoloLens (第 1 世代)</span><span class="sxs-lookup"><span data-stu-id="5dba5-110">HoloLens (1st gen)</span></span>

<span data-ttu-id="5dba5-111">HoloLens のコンテンツの対象とする (第 1 世代) を行う主に、[視線](gaze.md)ベクトル (光線の位置と、先頭のローテーションによって制御されます)。</span><span class="sxs-lookup"><span data-stu-id="5dba5-111">Targeting of content on HoloLens (1st gen) is done primarily with the [gaze](gaze.md) vector (a ray controlled by the position and rotation of the head).</span></span> <span data-ttu-id="5dba5-112">これは、ほとんどの教育の必要のあるユーザーの直接入力の形式を提供します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-112">This provides a form of direct input for the user that needs little teaching.</span></span> <span data-ttu-id="5dba5-113">ただし、ユーザーはあるカーソルにより、ユーザーが現在対象とする点を知っているので、正確な対象化の視線の先のマークされていない、センターの使用が困難です。</span><span class="sxs-lookup"><span data-stu-id="5dba5-113">However, users have difficulty using an unmarked center of gaze for precise targeting so a cursor ensures users know the point they are currently targeting.</span></span> 


## <a name="positioning"></a><span data-ttu-id="5dba5-114">配置</span><span class="sxs-lookup"><span data-stu-id="5dba5-114">Positioning</span></span>

<span data-ttu-id="5dba5-115">一般に、インジケーターは、ヘッドの移動と 1 対 1 の比率約で移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-115">In general, the indicator should move in approximately a 1:1 ratio with head movement.</span></span> <span data-ttu-id="5dba5-116">向上 (補強または移動著しく時間がかかりました) は、意図的なものの整備士として使用される可能性も予期せずに使用する場合のユーザーの問題により場合がある (わずかな 'lag' に関する問題を回避するために、カーソルの推奨があることに注意してください完全に表示、ロックされているコンテンツ)。</span><span class="sxs-lookup"><span data-stu-id="5dba5-116">There are some cases where gain (augmenting or diminishing movement noticeably) might be used as an intentional mechanic, but it will cause trouble for users if used unexpectedly (note that there is a tiny bit of 'lag' recommended for the cursor to avoid issues with fully display-locked content).</span></span> <span data-ttu-id="5dba5-117">最も重要なは、経験する必要があります「言う」- のカーソル位置の表記で、平滑化の向上、磁力場合またはその他の効果が含まれていますと、システムも表示されます、カーソルと、位置のシステムの理解は、任意の場所効果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5dba5-117">Most importantly though, experiences should be "honest" in the representation of cursor position - if smoothing, magnetism, gain, or other effects are included, the system should still show the cursor wherever the system's understanding of position is, with those effects included.</span></span> <span data-ttu-id="5dba5-118">カーソルは、システムのできることをユーザーに求める方法または対話ことはできませんをシステムに伝えるのユーザーの方法ではありません。</span><span class="sxs-lookup"><span data-stu-id="5dba5-118">The cursor is the system's way of telling the user what they can or can't interact with, not the user's way of telling the system.</span></span>

<span data-ttu-id="5dba5-119">ユーザーを対象にできますらしく任意の要素の深さの値内のインジケーターのロックする必要がありますが理想的です。</span><span class="sxs-lookup"><span data-stu-id="5dba5-119">The indicator should ideally lock in depth to whatever elements the user can plausibly target.</span></span> <span data-ttu-id="5dba5-120">これは、可能性が画面のロックがある場合[空間マッピング](spatial-mapping.md)メッシュまたはロックの「フローティング」の UI 要素の深さを理解しているユーザーを支援するはリアルタイムで対話することができます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-120">This may mean surface-locking if there is some [Spatial Mapping](spatial-mapping.md) mesh or locking to the depth of any "floating" UI elements, to help the user understand what they can interact with in real-time.</span></span>

## <a name="cursor-design-principles"></a><span data-ttu-id="5dba5-121">カーソルの設計原則</span><span class="sxs-lookup"><span data-stu-id="5dba5-121">Cursor design principles</span></span>

### <a name="always-present"></a><span data-ttu-id="5dba5-122">常に存在します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-122">Always present</span></span>
* <span data-ttu-id="5dba5-123">カーソルが常に存在することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5dba5-123">We recommend that the cursor is always present.</span></span>
* <span data-ttu-id="5dba5-124">場合は、ユーザーは、失われたいるし、カーソルを見つけることができません。</span><span class="sxs-lookup"><span data-stu-id="5dba5-124">If the user can't find the cursor, then they're lost.</span></span>
* <span data-ttu-id="5dba5-125">この例外には、ユーザーの準最適なエクスペリエンスを提供、カーソルを持つので、インスタンスです。</span><span class="sxs-lookup"><span data-stu-id="5dba5-125">Exceptions to this are instances where having a cursor provides a suboptimal experience for the user.</span></span> <span data-ttu-id="5dba5-126">たとえばは、ユーザーがビデオを見ているときです。</span><span class="sxs-lookup"><span data-stu-id="5dba5-126">An example is when a user is watching a video.</span></span> <span data-ttu-id="5dba5-127">カーソルは常に、ビデオの中では、この時点で望ましくないになります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-127">The cursor becomes undesirable at this point as it's in the middle of the video all the time.</span></span> <span data-ttu-id="5dba5-128">これは、シナリオがカーソルをユーザーがある、手動アクションを実行したいという願望を示すときにのみ表示されることを検討することがあります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-128">This is a scenario where you may consider making the cursor only visible when the user has their hand up indicating a desire to take action.</span></span> <span data-ttu-id="5dba5-129">それ以外の場合、ビデオに表示されていません。</span><span class="sxs-lookup"><span data-stu-id="5dba5-129">Otherwise, it's not visible on the video.</span></span>

### <a name="cursor-scale"></a><span data-ttu-id="5dba5-130">カーソルのスケール</span><span class="sxs-lookup"><span data-stu-id="5dba5-130">Cursor scale</span></span>
* <span data-ttu-id="5dba5-131">カーソルをコンテンツの表示し、対話を簡単にできるように、利用可能なターゲットを超えることがあります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-131">The cursor should be no larger than the available targets, allowing users to easily interact with and view the content.</span></span>
* <span data-ttu-id="5dba5-132">によって、エクスペリエンスを作成する、ユーザー次のようにカーソルをスケール重要な考慮事項も。</span><span class="sxs-lookup"><span data-stu-id="5dba5-132">Depending on the experience you create, scaling the cursor as the user looks around is also an important consideration.</span></span> <span data-ttu-id="5dba5-133">など、ユーザーはさらに、お客様のエクスペリエンスにおそらくカーソルにならないように小さすぎるようにその失われます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-133">For example, as the user looks further away in your experience perhaps the cursor should not become too small such that its lost.</span></span>
* <span data-ttu-id="5dba5-134">カーソルをスケーリングするときに、有機的な感情を付けることがスケール アップに論理的なアニメーションを適用することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="5dba5-134">When scaling the cursor, consider applying a soft animation to it as it scales giving it an organic feeling.</span></span>
* <span data-ttu-id="5dba5-135">コンテンツの障害を回避します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-135">Avoid obstructing content.</span></span> <span data-ttu-id="5dba5-136">ホログラムはどのようなこと、エクスペリエンスを覚えやすいとから離れた場所にカーソルを考慮しない必要があります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-136">Holograms are what make the experience memorable and the cursor should not be taking away from them.</span></span>

### <a name="directionless-cursor"></a><span data-ttu-id="5dba5-137">間接カーソル</span><span class="sxs-lookup"><span data-stu-id="5dba5-137">Directionless cursor</span></span>
* <span data-ttu-id="5dba5-138">1 つの適切なカーソルなしですが、トーラスまたは別のもののような方向性の図形を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5dba5-138">Although there is no one right cursor shape, we recommend that you use a directionless shape like a torus or something else.</span></span> <span data-ttu-id="5dba5-139">いくつかの方向を示すカーソル (例: 従来の矢印カーソル) 常にその方法を検索するユーザーが混乱する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-139">A cursor that points in some direction (ex: a traditional arrow cursor) might confuse the user to always look that way.</span></span>
* <span data-ttu-id="5dba5-140">この例外は、ユーザーに相互作用の命令を通信するために、カーソルを使用する場合です。</span><span class="sxs-lookup"><span data-stu-id="5dba5-140">An exception to this is when using the cursor to communicate interaction instruction to the user.</span></span> <span data-ttu-id="5dba5-141">たとえば、Windows Holographic のシェルでホログラムをスケーリングするときに、カーソルは一時的にホログラムをスケールする、手の形を移動する方法を指示する矢印に該当します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-141">For example, when scaling holograms in the Windows Holographic shell, the cursor temporarily includes arrows that help instruct the user on how to move their hand to scale the hologram.</span></span>

### <a name="look-and-feel"></a><span data-ttu-id="5dba5-142">ルック アンド フィール</span><span class="sxs-lookup"><span data-stu-id="5dba5-142">Look and feel</span></span>
* <span data-ttu-id="5dba5-143">ドーナツまたはトーラス カーソル動作の多くのアプリケーションから形成されました。</span><span class="sxs-lookup"><span data-stu-id="5dba5-143">A donut or torus shaped cursor works for a lot of applications.</span></span>
* <span data-ttu-id="5dba5-144">色と図形を作成するエクスペリエンスを最も良く表すものを選択します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-144">Pick a color and shape that best represents the experience you are creating.</span></span>
* <span data-ttu-id="5dba5-145">カーソルは、特にしやすい[色の分離](hologram-stability.md#color-separation)します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-145">Cursors are especially prone to [color separation](hologram-stability.md#color-separation).</span></span>
* <span data-ttu-id="5dba5-146">バランスの取れた不透明度の小さいカーソル状態に保ちます役に立つビジュアルの階層を占有することなしです。</span><span class="sxs-lookup"><span data-stu-id="5dba5-146">A small cursor with balanced opacity keeps it informative without dominating the visual hierarchy.</span></span>
* <span data-ttu-id="5dba5-147">できなければの影や、カーソルの背後にある主なトピックを使用して、コンテンツの妨げし、目的から注意をそらす可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-147">Be cognizant of using shadows or highlights behind your cursor as they might obstruct content and distract from the purpose.</span></span>
* <span data-ttu-id="5dba5-148">これにより、ユーザー システムが探す場所を表示できることに気がすることも、カーソルに合わせて配置する必要があり、アプリで、サーフェスをハグ、システムがその周囲に注意してください。</span><span class="sxs-lookup"><span data-stu-id="5dba5-148">Cursors should align to and hug the surfaces in your app, this will give the user a feeling that the system can see where they are looking, but also that the system is aware of their surroundings.</span></span>
* <span data-ttu-id="5dba5-149">たとえば、Windows Holographic OS では、カーソルは、ユーザーの世界では、ユーザーはホログラムで直接検索する場合でも、世界中の認識の気の作成のサーフェスに配置.</span><span class="sxs-lookup"><span data-stu-id="5dba5-149">For example, in the Windows Holographic OS, the cursor aligns to the surfaces of the user's world, creating a feeling of awareness of the world even when the user isn't looking directly at a hologram..</span></span>
* <span data-ttu-id="5dba5-150">近接磁気内にある場合に対話型の要素にカーソルをロックします。</span><span class="sxs-lookup"><span data-stu-id="5dba5-150">Magnetically locking the cursor to an interactive element when it is within close proximity.</span></span> <span data-ttu-id="5dba5-151">これにより、選択アクションを実行するときに、その要素とそのユーザーが操作の信頼性を向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-151">This can help improve confidence that user will interact with that element when they perform a selection action.</span></span>

### <a name="visual-cues"></a><span data-ttu-id="5dba5-152">視覚的な合図</span><span class="sxs-lookup"><span data-stu-id="5dba5-152">Visual cues</span></span>
* <span data-ttu-id="5dba5-153">多くの情報は、世界では、ホログラムで詳細を追加しています。</span><span class="sxs-lookup"><span data-stu-id="5dba5-153">There is a lot of information in our world and with holograms we are adding more information.</span></span> <span data-ttu-id="5dba5-154">カーソルは、重要なは、ユーザーに通知する優れた方法です。</span><span class="sxs-lookup"><span data-stu-id="5dba5-154">A cursor is a great way of communicating to the user what is important.</span></span>
* <span data-ttu-id="5dba5-155">エクスペリエンスは、1 つホログラムにフォーカスがある場合、おそらくカーソル整列し、ホログラムと変更が、そのホログラムから確認するときを図形 hugs のみ。</span><span class="sxs-lookup"><span data-stu-id="5dba5-155">If your experience is focused on a single hologram, then perhaps your cursor aligns and hugs only that hologram and changes shape when you look away from that hologram.</span></span> <span data-ttu-id="5dba5-156">これには、ホログラムは特殊で、それに対処可能なことをユーザーに伝達できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-156">This can convey to the user that the hologram is special and they can interact with it.</span></span>
* <span data-ttu-id="5dba5-157">アプリケーションでは、空間マッピングを使用する場合、カーソルでした配置し、ハグが見つかるすべての画面。</span><span class="sxs-lookup"><span data-stu-id="5dba5-157">If your application uses spatial mapping, then your cursor could align and hug every surface it sees.</span></span> <span data-ttu-id="5dba5-158">これにより、フィードバック、ユーザーにその HoloLens と、アプリケーションは、容量を確認できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-158">This gives feedback to the users that HoloLens and your application can see their space.</span></span>
* <span data-ttu-id="5dba5-159">これらの操作では、ホログラムは、実際のところ、という事実を強調するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-159">These things help reinforce the fact that holograms are real and in our world.</span></span> <span data-ttu-id="5dba5-160">実数部と仮想のギャップを埋めるのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-160">They help bridge the gap between real and virtual.</span></span>
* <span data-ttu-id="5dba5-161">急ぎのカーソルに何がない場合ホログラムまたはサーフェスに表示します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-161">Have an idea of what the cursor should do when there are no holograms or surfaces in view.</span></span> <span data-ttu-id="5dba5-162">1 つのオプションには、ユーザーの前に事前に定義された距離に配置することです。</span><span class="sxs-lookup"><span data-stu-id="5dba5-162">Placing it at a predetermined distance in front of the user is one option.</span></span>

## <a name="cursor-feedback"></a><span data-ttu-id="5dba5-163">カーソルからのフィードバック</span><span class="sxs-lookup"><span data-stu-id="5dba5-163">Cursor feedback</span></span>

<span data-ttu-id="5dba5-164">述べた常に存在する、いくつかの重要なビットの情報を伝達するために、カーソルを使用すると、カーソルがあることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5dba5-164">As we mentioned it is good practice to have the cursor always be present, as you can use the cursor to convey some important bits of information.</span></span>

### <a name="possible-actions"></a><span data-ttu-id="5dba5-165">実行可能なアクション</span><span class="sxs-lookup"><span data-stu-id="5dba5-165">Possible actions</span></span>
* <span data-ttu-id="5dba5-166">ユーザーはホログラムで gazing し、そのホログラム上にカーソルが、そのホログラムで可能なアクションを伝達するために、カーソルを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-166">As the user is gazing at a hologram and the cursor is on that hologram, you could use the cursor to convey possible actions on that hologram.</span></span>
* <span data-ttu-id="5dba5-167">たとえばを購入するアイテムや、場合によっては、そのホログラムをスケーリングするカーソルでは、アイコンを表示できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-167">You could display an icon on the cursor that the user can for example purchase that item or perhaps scale that hologram.</span></span> <span data-ttu-id="5dba5-168">または、でも、といった簡単なもの、ホログラムで求めることができます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-168">Or even something as simple like the hologram can be tapped on.</span></span>
* <span data-ttu-id="5dba5-169">のみをユーザーに意味がある場合は、カーソル上で追加情報を追加します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-169">Only add extra information on the cursor if it means something to the user.</span></span> <span data-ttu-id="5dba5-170">それ以外の場合、ユーザーは、状態の変更に気付かないか、またはカーソルが混同します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-170">Otherwise, users might either not notice the state changes or get confused by the cursor.</span></span>

### <a name="input-state"></a><span data-ttu-id="5dba5-171">入力の状態</span><span class="sxs-lookup"><span data-stu-id="5dba5-171">Input state</span></span>
* <span data-ttu-id="5dba5-172">ユーザーの入力の状態を表示するのに、カーソルを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-172">We could use the cursor to display the user's input state.</span></span> <span data-ttu-id="5dba5-173">たとえば、システムが、手の形の状態を表示するかどうかを示すアイコンを表示しますでした。</span><span class="sxs-lookup"><span data-stu-id="5dba5-173">For example, we could display an icon telling the user if the system sees their hand state.</span></span> <span data-ttu-id="5dba5-174">これにより、ユーザー、アプリケーションをユーザーがアクションを実行する準備が知っていること。</span><span class="sxs-lookup"><span data-stu-id="5dba5-174">This will tell the user that the application knows the user is ready to take action.</span></span>
* <span data-ttu-id="5dba5-175">ユーザーの利用可能な音声コマンドがあることに注意してください、カーソルも使用できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-175">We could also use the cursor to make the user aware that there is a voice command available.</span></span> <span data-ttu-id="5dba5-176">または、おそらく、音声コマンドがシステムによって音がユーザーに通知するには、一時的にカーソルの色を変更します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-176">Or perhaps change the color of the cursor momentarily to tell the user that the voice command was heard by the system.</span></span>

<span data-ttu-id="5dba5-177">これらのカーソルの状態は、さまざまな方法で実装できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-177">These different cursor states can be implemented in different ways.</span></span> <span data-ttu-id="5dba5-178">ステート マシンのようにカーソルをシミュレートしてこれらのさまざまな状態を実装する場合があります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-178">You might implement these different states by modeling the cursor like a state machine.</span></span> <span data-ttu-id="5dba5-179">次に、例を示します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-179">For example:</span></span>
* <span data-ttu-id="5dba5-180">アイドル状態では、既定のカーソルを表示します。</span><span class="sxs-lookup"><span data-stu-id="5dba5-180">Idle state is where you show the default cursor.</span></span>
* <span data-ttu-id="5dba5-181">準備完了状態は、準備完了の位置にユーザーの手を検出した場合です。</span><span class="sxs-lookup"><span data-stu-id="5dba5-181">Ready state is when you have detected the user's hand in the ready position.</span></span>
* <span data-ttu-id="5dba5-182">対話状態は、ユーザーが特定の操作を実行する場合です。</span><span class="sxs-lookup"><span data-stu-id="5dba5-182">Interaction state is when the user is performing a particular interaction.</span></span>
* <span data-ttu-id="5dba5-183">可能なアクションの状態は、ホログラムで実行できる実行可能なアクションを伝達する場合です。</span><span class="sxs-lookup"><span data-stu-id="5dba5-183">Possible Actions state is when you convey possible actions that can be performed on a hologram.</span></span>

<span data-ttu-id="5dba5-184">さまざまなアート アセットを表示するには、さまざまな状態が検出されるように、スキンできない方法でこれらの状態を実装できます。</span><span class="sxs-lookup"><span data-stu-id="5dba5-184">You could also implement these states in a skin-able manner such that you can display different art assets when different states are detected.</span></span>

## <a name="going-cursor-free"></a><span data-ttu-id="5dba5-185">「カーソルのない」に移動</span><span class="sxs-lookup"><span data-stu-id="5dba5-185">Going "cursor-free"</span></span>

<span data-ttu-id="5dba5-186">カーソルなしの設計を immersion の意味は、エクスペリエンスの重要なコンポーネントと相互作用を伴う (視線、ジェスチャから) を対象とする非常に正確必要としない場合にのみお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5dba5-186">Designing without a cursor is recommended only when the sense of immersion is a key component of an experience, and interactions that involve targeting (through gaze and gesture) do not require great precision.</span></span> <span data-ttu-id="5dba5-187">システムは、通常により満たされているカーソルを対象のシステムの理解に継続的なフィードバックをユーザーに提供して、システムに各自の意志を自信を持って通信を支援できますニーズを満たすもする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-187">The system must still meet the needs that are normally met by a cursor though - providing users with continuous feedback on the system's understanding of their targeting and helping them to confidently communicate their intentions to the system.</span></span> <span data-ttu-id="5dba5-188">これは、その他の顕著な状態の変更によって達成可能な可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5dba5-188">This may be achievable through other noticeable state changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="5dba5-189">関連項目</span><span class="sxs-lookup"><span data-stu-id="5dba5-189">See also</span></span>
* [<span data-ttu-id="5dba5-190">ジェスチャ</span><span class="sxs-lookup"><span data-stu-id="5dba5-190">Gestures</span></span>](gestures.md)
* [<span data-ttu-id="5dba5-191">視線の先を対象とします。</span><span class="sxs-lookup"><span data-stu-id="5dba5-191">Gaze targeting</span></span>](gaze-targeting.md)