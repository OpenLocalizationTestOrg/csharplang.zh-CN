---
ms.openlocfilehash: 97f4a97a674e17870f1d24e35258c4f79c559eb2
ms.sourcegitcommit: 55811c551095ea9ab89baf1144ac0cf7fb1c5df8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/01/2019
ms.locfileid: "57253859"
---
<properties
pageTitle="最重要的常见计算问题"
description="基于前计算问题的工作流文档菜单"        
service="microsoft.compute"
resource="virtualmachines"
authors="gamore"
displayOrder=""
articleId="7bd33a4a-8d59-4f16-a965-f1ac9deb730e"
selfHelpType="diagnoseandsolvev2"
resourceTags="linux"
productPesId="15571"
cloudEnvironments="public"
/>
---
{
    "$schema": "SelfHelpContent",
    "commonProblems": [
        {
            "title": "我无法连接到我的虚拟机",
            "description": "Discover issues that may be affecting connectivity to your VM due to either  platform issue or VM issue",
            "category": "Connectivity",
            "searchTags": "connectivity, rdp",
            "supportTopicId": "4354354565",
            "symptomId": "cannotrdpazureportalinsight"
        },
        {
            "title": "我不能重新启动/重新启动我的虚拟机",
            "description": "Discover issues that may be affecting connectivity to your VM due to either  platform issue or VM issue",
            "category": "Connectivity",
            "searchTags": "restart, reboot",
            "supportTopicId": "4354354567"
        },
        {
            "title": "我的虚拟机运行速度缓慢",
            "description": "Discover issues that may be affecting connectivity to your VM due to either  platform issue or VM issue",
            "category": "Performance",
            "searchTags": "performance, vm",
            "supportTopicId": "4354354565"
        },
        {
            "title": "如何重置我的虚拟机的密码？",
            "description": "Discover issues that may be affecting connectivity to your VM due to either  platform issue or VM issue",
            "category": "Reset",
            "supportTopicId": "4354354565"
        }
    ],
    "troubleshootingTools": [
        {
            "title": "重新部署虚拟机",
            "description": "Migrate this virtual machine to a different host to resolve connectivity issues",
            "newTagExpiryDate": "4/14/2019",
            "category": "Connectivity",
            "searchTags": "deployment, rdp",
            "type": "tool",
            "bladeLink": {
                "extensionName": "Microsoft_Azure_Compute",
                "bladeName": "VirtualMachineRedeployViewModel",
                "parameters": [
                    {
                        "name": "id",
                        "value": "$resourceId"
                    }
                ]
            }
        },
        {
            "title": "无法连接到虚拟机",
            "description": "Discover issues that may be affecting connectivity to your VM due to either  platform issue or VM issue",
            "newTagExpiryDate": "",
            "type": "insight",
            "searchTags": "connectvity, rdp",
            "category": "Connectivity",
            "supportTopicId": "4354354565",
            "symptomId": "cannotrdpazureportalinsight"
        }
    ]
}
---
