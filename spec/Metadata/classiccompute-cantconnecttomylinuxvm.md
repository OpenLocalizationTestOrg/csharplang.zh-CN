---
ms.openlocfilehash: 32610e9ef1fce157dd3d9480867948d25feac2ce
ms.sourcegitcommit: fed965b15069147176339f9d0d33ff38f0b95f6a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/23/2019
ms.locfileid: "57253844"
---
<properties
    pageTitle="我无法连接到我的 VM"
    description="我无法连接到我的 VM "
    service="microsoft.classiccompute"
    resource="virtualmachines"
    authors="ScottAzure"
    ms.author="scotro"
    displayOrder="2"
    selfHelpType="resource"
    supportTopicIds="32615531,32615526"
    resourceTags="linux,redhat,Ubuntu"
    productPesIds="16470,15797,15571,16454"
    cloudEnvironments="public"
    articleId="420298f8-b3fb-49f2-b359-f7cdf357901c"
    category="连接"
    searchTags="无法连接，无法连接，连接、 vm、 rdp"
 />

# <a name="i-cant-connect-to-my-vm"></a><span data-ttu-id="815d3-105">我无法连接到我的 VM</span><span class="sxs-lookup"><span data-stu-id="815d3-105">I can't connect to my VM</span></span>

<span data-ttu-id="815d3-106">4 共 5 客户解决其 VM 连接性问题使用以下步骤。</span><span class="sxs-lookup"><span data-stu-id="815d3-106">4 out of 5 customers resolved their VM connectivity issue using the below steps.</span></span><br>

## <a name="recommended-steps"></a><span data-ttu-id="815d3-107">**建议的步骤**</span><span class="sxs-lookup"><span data-stu-id="815d3-107">**Recommended Steps**</span></span>

<span data-ttu-id="815d3-108">若要解决常见问题，请尝试一个或多个以下方法：</span><span class="sxs-lookup"><span data-stu-id="815d3-108">To resolve common issues, try one or more of the following methods:</span></span><br>

1. <span data-ttu-id="815d3-109">验证 VM 是否通过查看 VM 的运行[控制台日志或屏幕截图](data-blade:Microsoft_Azure_Classic_Compute.VirtualMachineSerialConsoleLogBlade.id.$resourceId)。</span><span class="sxs-lookup"><span data-stu-id="815d3-109">Verify if your VM is running by viewing your VM's [console log or screenshot](data-blade:Microsoft_Azure_Classic_Compute.VirtualMachineSerialConsoleLogBlade.id.$resourceId).</span></span><br>

    * <span data-ttu-id="815d3-110">查看 FSTAB （文件系统表）、 FSCK （文件系统一致性） 或网络等日志中的错误。</span><span class="sxs-lookup"><span data-stu-id="815d3-110">Review errors in logs such as FSTAB (file systems table), FSCK (file system consistency), or networking.</span></span><br>

2. <span data-ttu-id="815d3-111">单击[此处](data-blade:microsoft_azure_network.verifyipflowblade.vmId.$resourceId)以确保网络安全组允许流量。</span><span class="sxs-lookup"><span data-stu-id="815d3-111">Click [here](data-blade:microsoft_azure_network.verifyipflowblade.vmId.$resourceId) to ensure that Network Security Group is allowing traffic.</span></span><br>
3. <span data-ttu-id="815d3-112">单击[此处](data-blade:microsoft_azure_network.NetworkWatcherConnectivityBlade.id.$resourceId)时尝试从 Azure 执行 SSH 连接问题进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="815d3-112">Click [here](data-blade:microsoft_azure_network.NetworkWatcherConnectivityBlade.id.$resourceId) to troubleshoot connectivity issues when trying SSH from Azure.</span></span><br>
4. <span data-ttu-id="815d3-113">[重置密码](data-blade:Microsoft_Azure_Classic_Compute.PasswordResetBlade.id.$resourceId)以解决身份验证错误。</span><span class="sxs-lookup"><span data-stu-id="815d3-113">[Reset password](data-blade:Microsoft_Azure_Classic_Compute.PasswordResetBlade.id.$resourceId) to address authentication errors.</span></span><br>
5. <span data-ttu-id="815d3-114">通过单击重新启动在 VM 资源边栏选项卡的顶部，重新启动虚拟机以解决启动问题。</span><span class="sxs-lookup"><span data-stu-id="815d3-114">Restart the virtual machine to address startup issues by clicking 'Restart' at the top of the VM resource blade.</span></span><br>
6. <span data-ttu-id="815d3-115">调整大小的 VM 通过在 VM 资源的设置边栏选项卡中单击大小来解决主机问题。</span><span class="sxs-lookup"><span data-stu-id="815d3-115">Resize the VM to fix host issues by clicking 'Size' in the Settings blade of the VM resource.</span></span><br>
7. <span data-ttu-id="815d3-116">重置 SSH 配置以解决任何 SSH 问题[使用 CLI](https://docs.microsoft.com/azure/virtual-machines/linux/classic/reset-access-classic#sshconfigresetcli)</span><span class="sxs-lookup"><span data-stu-id="815d3-116">Reset the SSH configuration to fix any SSH issues [using CLI](https://docs.microsoft.com/azure/virtual-machines/linux/classic/reset-access-classic#sshconfigresetcli)</span></span>

## <a name="recommended-documents"></a><span data-ttu-id="815d3-117">**建议的文档**</span><span class="sxs-lookup"><span data-stu-id="815d3-117">**Recommended Documents**</span></span>

* [<span data-ttu-id="815d3-118">SSH 错误的详细故障排除</span><span class="sxs-lookup"><span data-stu-id="815d3-118">Detailed troubleshooting of SSH errors</span></span>](https://azure.microsoft.com/documentation/articles/virtual-machines-troubleshoot-ssh-connections/#detailed-troubleshooting-of-ssh-errors)<br>
* [<span data-ttu-id="815d3-119">自动执行 Linux VM 自定义任务使用自定义脚本扩展</span><span class="sxs-lookup"><span data-stu-id="815d3-119">Automate Linux VM Customization Tasks using Custom Script Extension</span></span>](https://azure.microsoft.com/blog/automate-linux-vm-customization-tasks-using-customscript-extension)
