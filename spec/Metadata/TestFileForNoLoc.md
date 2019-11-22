---
title: 使用 Azure 顾问降低服务成本 |Microsoft Docs
description: 使用 Azure 顾问优化 Azure 部署的成本。
services: advisor
documentationcenter: NA
author: kasparks
ms.service: advisor
ms.topic: article
ms.date: 01/29/2019
ms.author: kasparks
ms.openlocfilehash: c8b5f84541bce641b60b5e0c55a8c701850b57f0
ms.sourcegitcommit: 5eac2b357ddc023f87e520e04cafde87796ee319
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2019
ms.locfileid: "6610234"
---
![Test1noicon](./image/Test1noicon.png)

# <a name="reduce-service-costs-using-azure-advisor"></a><span data-ttu-id="ce66e-104">使用 Azure 顾问降低服务成本</span><span class="sxs-lookup"><span data-stu-id="ce66e-104">Reduce service costs using Azure Advisor</span></span>

<span data-ttu-id="ce66e-105">顾问通过识别空闲和未充分利用的资源，帮助你优化和减少总体 Azure 支出。</span><span class="sxs-lookup"><span data-stu-id="ce66e-105">Advisor helps you optimize and reduce your overall Azure spend by identifying idle and underutilized resources.</span></span> <span data-ttu-id="ce66e-106">可以从顾问仪表板上的 "**成本**" 选项卡获取成本建议。</span><span class="sxs-lookup"><span data-stu-id="ce66e-106">You can get cost recommendations from the **Cost** tab on the Advisor dashboard.</span></span> <span data-ttu-id="ce66e-107">这是测试123。</span><span class="sxs-lookup"><span data-stu-id="ce66e-107">This is TEST 123.</span></span>

## <a name="optimize-virtual-machine-spend-by-resizing-or-shutting-down-underutilized-instances"></a><span data-ttu-id="ce66e-108">通过调整大小或关闭未充分利用的实例来优化虚拟机花费</span><span class="sxs-lookup"><span data-stu-id="ce66e-108">Optimize virtual machine spend by resizing or shutting down underutilized instances</span></span> 

<span data-ttu-id="ce66e-109">虽然某些应用程序方案在设计上可能导致低利用率，但你通常可以通过管理虚拟机的大小和数量来节省资金。</span><span class="sxs-lookup"><span data-stu-id="ce66e-109">Although certain application scenarios can result in low utilization by design, you can often save money by managing the size and number of your virtual machines.</span></span> <span data-ttu-id="ce66e-110">Advisor 会监视你的虚拟机使用情况7天，然后标识低利用率虚拟机。</span><span class="sxs-lookup"><span data-stu-id="ce66e-110">Advisor monitors your virtual machine usage for 7 days and then identifies low-utilization virtual machines.</span></span> <span data-ttu-id="ce66e-111">如果虚拟机的 CPU 利用率为5% 或更低，并且其网络利用率小于2%，或者当前工作负荷可由较小的虚拟机大小容纳，则会将虚拟机视为低利用率。这是不是就地测试。</span><span class="sxs-lookup"><span data-stu-id="ce66e-111">Virtual machines are considered low-utilization if their CPU utilization is 5% or less and their network utilization is less than 2% or if the current workload can be accommodated by a smaller virtual machine size.This is no-loc test.</span></span>

<span data-ttu-id="ce66e-112">顾问会显示继续运行虚拟机所需的估计成本，以便可以选择关闭虚拟机或调整其大小。</span><span class="sxs-lookup"><span data-stu-id="ce66e-112">Advisor shows you the estimated cost of continuing to run your virtual machine, so that you can choose to shut it down or resize it.</span></span>

<span data-ttu-id="ce66e-113">如果你想要更积极地识别使用不足的虚拟机，你可以基于每个订阅调整平均 CPU 使用率规则。</span><span class="sxs-lookup"><span data-stu-id="ce66e-113">If you want to be more aggressive at identifying underutilized virtual machines, you can adjust the average CPU utilization rule on a per subscription basis.</span></span>

## <a name="reduce-costs-by-eliminating-unprovisioned-expressroute-circuits"></a><span data-ttu-id="ce66e-114">消除未设置的 ExpressRoute 线路，从而降低成本</span><span class="sxs-lookup"><span data-stu-id="ce66e-114">Reduce costs by eliminating unprovisioned ExpressRoute circuits</span></span>

<span data-ttu-id="ce66e-115">顾问会确定提供程序状态为 "*未设置*" 的 ExpressRoute 线路超过一个月，如果不打算使用连接服务提供商来预配线路，则建议删除该线路。</span><span class="sxs-lookup"><span data-stu-id="ce66e-115">Advisor identifies ExpressRoute circuits that have been in the provider status of *Not Provisioned* for more than one month, and recommends deleting the circuit if you aren't planning to provision the circuit with your connectivity provider.</span></span>

## <a name="reduce-costs-by-deleting-or-reconfiguring-idle-virtual-network-gateways"></a><span data-ttu-id="ce66e-116">删除或重新配置空闲虚拟网络网关，降低成本</span><span class="sxs-lookup"><span data-stu-id="ce66e-116">Reduce costs by deleting or reconfiguring idle virtual network gateways</span></span>

<span data-ttu-id="ce66e-117">顾问标识在超过90天内空闲的虚拟网络入口。</span><span class="sxs-lookup"><span data-stu-id="ce66e-117">Advisor identifies virtual network gates that have been idle for over 90 days.</span></span> <span data-ttu-id="ce66e-118">由于这些网关按小时计费，因此，如果不想再使用它们，则应考虑重新配置或删除它们。</span><span class="sxs-lookup"><span data-stu-id="ce66e-118">Since these gateways are billed hourly, you should consider reconfiguring or deleting them if you don't intend to use them anymore.</span></span> 

## <a name="buy-reserved-virtual-machine-instances-to-save-money-over-pay-as-you-go-costs"></a><span data-ttu-id="ce66e-119">购买保留虚拟机实例，通过即用即付成本节省资金</span><span class="sxs-lookup"><span data-stu-id="ce66e-119">Buy reserved virtual machine instances to save money over pay-as-you-go costs</span></span>

<span data-ttu-id="ce66e-120">Advisor 将在过去30天内检查虚拟机的使用情况，并确定是否可以通过购买 Azure 保留来节省资金。</span><span class="sxs-lookup"><span data-stu-id="ce66e-120">Advisor will review your virtual machine usage over the last 30 days and determine if you could save money by purchasing an Azure reservation.</span></span> <span data-ttu-id="ce66e-121">顾问会向你显示最大限度地节省费用的区域和大小，并将向你显示购买预留的估计节省量。</span><span class="sxs-lookup"><span data-stu-id="ce66e-121">Advisor will show you the regions and sizes where you potentially have the most savings and will show you the estimated savings from purchasing reservations.</span></span> <span data-ttu-id="ce66e-122">借助 Azure 保留，你可以为虚拟机预先购买基本成本。</span><span class="sxs-lookup"><span data-stu-id="ce66e-122">With Azure reservations, you can pre-purchase the base costs for your virtual machines.</span></span> <span data-ttu-id="ce66e-123">折扣将自动应用于与预留大小和区域相同的新的或现有的 Vm。</span><span class="sxs-lookup"><span data-stu-id="ce66e-123">Discounts will automatically apply to new or existing VMs that have the same size and region as your reservations.</span></span> [<span data-ttu-id="ce66e-124">详细了解 Azure 保留 VM 实例。</span><span class="sxs-lookup"><span data-stu-id="ce66e-124">Learn more about Azure Reserved VM Instances.</span></span>](https://azure.microsoft.com/pricing/reserved-vm-instances/)

<span data-ttu-id="ce66e-125">顾问还会通知你你的保留实例将在未来30天到期。</span><span class="sxs-lookup"><span data-stu-id="ce66e-125">Advisor will also notify you of reserved instances that you have that will expire in the next 30 days.</span></span> <span data-ttu-id="ce66e-126">建议你购买新的预订实例，以避免支付即用即付定价。</span><span class="sxs-lookup"><span data-stu-id="ce66e-126">It will recommend that you purchase new reserved instances to avoid paying pay-as-you-go pricing.</span></span>

## <a name="delete-unassociated-public-ip-addresses-to-save-money"></a><span data-ttu-id="ce66e-127">删除未关联的公共 IP 地址以节省资金</span><span class="sxs-lookup"><span data-stu-id="ce66e-127">Delete unassociated public IP addresses to save money</span></span>

<span data-ttu-id="ce66e-128">顾问标识当前不与 Azure 资源（例如负载均衡器或 Vm）关联的公共 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ce66e-128">Advisor identifies public IP addresses that are not currently associated to Azure resources such as Load Balancers or VMs.</span></span> <span data-ttu-id="ce66e-129">这些公共 IP 地址附带了一个名义费用。</span><span class="sxs-lookup"><span data-stu-id="ce66e-129">These public IP addresses come with a nominal charge.</span></span> <span data-ttu-id="ce66e-130">如果你不打算使用它们，则删除它们可能会节省成本。</span><span class="sxs-lookup"><span data-stu-id="ce66e-130">If you do not plan to use them, deleting them can result in cost savings.</span></span>

## <a name="how-to-access-cost-recommendations-in-azure-advisor"></a><span data-ttu-id="ce66e-131">如何访问 Azure 顾问中的成本建议</span><span class="sxs-lookup"><span data-stu-id="ce66e-131">How to access Cost recommendations in Azure Advisor</span></span>

:::image type="complex"  alt-text="这是一个复杂的图像测试功能，适用于图像 SxS 行为" source="./image/Test1noicon.png"::: 
<span data-ttu-id="ce66e-133">这是针对 SxS 的复杂映像测试功能的日志说明，这是 SxS 多行 testing1 :::image-end:::</span><span class="sxs-lookup"><span data-stu-id="ce66e-133">this is a log description for complex image testing feature for SxS This is SxS multiline testing1 :::image-end:::</span></span>

1. <span data-ttu-id="ce66e-134">登录到[Azure 门户](https://portal.azure.com)，然后打开[Advisor](https://aka.ms/azureadvisordashboard)。</span><span class="sxs-lookup"><span data-stu-id="ce66e-134">Sign in to the [Azure portal](https://portal.azure.com), and then open [Advisor](https://aka.ms/azureadvisordashboard).</span></span>
<span data-ttu-id="ce66e-135">:::icon source="image\Test123.png":::这是图标源测试，这是下一行的测试</span><span class="sxs-lookup"><span data-stu-id="ce66e-135">:::icon source="image\Test123.png":::This is icon source test This is test of next line</span></span>

2.  <span data-ttu-id="ce66e-136">在顾问仪表板上，单击 "**成本**" 选项卡。这是一个 :::no-loc text="TEST for inline lock":::，用于查看是否将删除 "测试内联位置" 或将其作为标记进行放置。</span><span class="sxs-lookup"><span data-stu-id="ce66e-136">On the Advisor dashboard, click the **Cost** tab. This is a :::no-loc text="TEST for inline lock"::: to see if the "TEST for inline loc" will be removed or put as a tag.</span></span>

:::image source="https://portal.azure.com" alt-text="这是图像源测试":::
<span data-ttu-id="ce66e-138">TLong 说明开始。顾问标识当前不与 Azure 资源（例如负载均衡器或 Vm）关联的公共 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ce66e-138">TLong Description start.Advisor identifies public IP addresses that are not currently associated to Azure resources such as Load Balancers or VMs.</span></span> <span data-ttu-id="ce66e-139">这些公共 IP 地址附带了一个名义费用。</span><span class="sxs-lookup"><span data-stu-id="ce66e-139">These public IP addresses come with a nominal charge.</span></span> <span data-ttu-id="ce66e-140">如果你不打算使用它们，则删除它们可能会节省成本。</span><span class="sxs-lookup"><span data-stu-id="ce66e-140">If you do not plan to use them, deleting them can result in cost savings.</span></span>
<span data-ttu-id="ce66e-141">长说明结束 :::image-end:::这是图像结束</span><span class="sxs-lookup"><span data-stu-id="ce66e-141">Long description end :::image-end:::This is image end</span></span>

::: image source= "./image/Test1noicon.png" alt-text="space teating":::

:::image type="complex" source="./image/Test1noicon.png" alt-text="这是一个用于 contoso-scope2 的复杂映像测试功能" loc-scope="Azure"::: 
<span data-ttu-id="ce66e-143">这是针对 contoso-scope2 的复杂映像测试功能的日志说明，这是多行 testing2 :::image-end:::</span><span class="sxs-lookup"><span data-stu-id="ce66e-143">this is a log description for complex image testing feature for loc-scope2 This is multiline testing2 :::image-end:::</span></span>

## <a name="next-steps"></a><span data-ttu-id="ce66e-144">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ce66e-144">Next steps</span></span>

<span data-ttu-id="ce66e-145">若要了解有关顾问建议的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="ce66e-145">To learn more about Advisor recommendations, see:</span></span>
* [<span data-ttu-id="ce66e-146">Advisor 简介</span><span class="sxs-lookup"><span data-stu-id="ce66e-146">Introduction to Advisor</span></span>](advisor-overview.md)
* [<span data-ttu-id="ce66e-147">入门</span><span class="sxs-lookup"><span data-stu-id="ce66e-147">Get Started</span></span>](advisor-get-started.md)
* [<span data-ttu-id="ce66e-148">顾问性能建议</span><span class="sxs-lookup"><span data-stu-id="ce66e-148">Advisor Performance recommendations</span></span>](advisor-cost-recommendations.md)
* [<span data-ttu-id="ce66e-149">顾问高可用性建议</span><span class="sxs-lookup"><span data-stu-id="ce66e-149">Advisor High Availability recommendations</span></span>](advisor-cost-recommendations.md)
* [<span data-ttu-id="ce66e-150">顾问安全建议</span><span class="sxs-lookup"><span data-stu-id="ce66e-150">Advisor Security recommendations</span></span>](advisor-cost-recommendations.md)
