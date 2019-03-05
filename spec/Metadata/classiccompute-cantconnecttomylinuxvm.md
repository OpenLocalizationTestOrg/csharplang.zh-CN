---
ms.openlocfilehash: 32610e9ef1fce157dd3d9480867948d25feac2ce
ms.sourcegitcommit: 55811c551095ea9ab89baf1144ac0cf7fb1c5df8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2019
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

# <a name="i-cant-connect-to-my-vm"></a>我无法连接到我的 VM

4 共 5 客户解决其 VM 连接性问题使用以下步骤。<br>

## <a name="recommended-steps"></a>**建议的步骤**

若要解决常见问题，请尝试一个或多个以下方法：<br>

1. 验证 VM 是否通过查看 VM 的运行[控制台日志或屏幕截图](data-blade:Microsoft_Azure_Classic_Compute.VirtualMachineSerialConsoleLogBlade.id.$resourceId)。<br>

    * 查看 FSTAB （文件系统表）、 FSCK （文件系统一致性） 或网络等日志中的错误。<br>

2. 单击[此处](data-blade:microsoft_azure_network.verifyipflowblade.vmId.$resourceId)以确保网络安全组允许流量。<br>
3. 单击[此处](data-blade:microsoft_azure_network.NetworkWatcherConnectivityBlade.id.$resourceId)时尝试从 Azure 执行 SSH 连接问题进行故障排除。<br>
4. [重置密码](data-blade:Microsoft_Azure_Classic_Compute.PasswordResetBlade.id.$resourceId)以解决身份验证错误。<br>
5. 通过单击重新启动在 VM 资源边栏选项卡的顶部，重新启动虚拟机以解决启动问题。<br>
6. 调整大小的 VM 通过在 VM 资源的设置边栏选项卡中单击大小来解决主机问题。<br>
7. 重置 SSH 配置以解决任何 SSH 问题[使用 CLI](https://docs.microsoft.com/azure/virtual-machines/linux/classic/reset-access-classic#sshconfigresetcli)

## <a name="recommended-documents"></a>**建议的文档**

* [SSH 错误的详细故障排除](https://azure.microsoft.com/documentation/articles/virtual-machines-troubleshoot-ssh-connections/#detailed-troubleshooting-of-ssh-errors)<br>
* [自动执行 Linux VM 自定义任务使用自定义脚本扩展](https://azure.microsoft.com/blog/automate-linux-vm-customization-tasks-using-customscript-extension)
