---
title: 远程调试器下载
description: 远程调试器的下载链接
services: ''
author: mikejo5000
ms.service: ''
ms.topic: include
ms.date: 05/23/2018
ms.author: mikejo
ms.custom: include file
ms.openlocfilehash: 491b01d87e4f1a9980143e9ffcc501b3cda7c922
ms.sourcegitcommit: 5b767247b3d819a99deb0dbce729a0562b9654ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2018
ms.locfileid: "39189223"
---
1.  在设备或服务器您想要调试的计算机 （而不运行 Visual Studio 的计算机），获取远程工具的正确版本。

    |版本|链接|说明|
    |-|-|-|
    |Visual Studio 2017 （最新版本）|[远程工具](https://visualstudio.microsoft.com/downloads/?q=remote+tools#remote-tools-for-visual-studio-2017)|远程工具的最新版本是与所有 Visual Studio 2017 版本兼容。 始终下载匹配您设备的操作系统 (x 86、 x64、 或 ARM64） 的版本。 在 Windows 服务器上，请参阅[取消阻止文件下载](../../debugger/remote-debugging-unblock-file-download.md)有关帮助下载的远程工具。|
    |Visual Studio 2015|[远程工具](https://my.visualstudio.com/Downloads?q=remote%20tools%20visual%20studio%202015)|Visual Studio 2015 远程工具可从 My.VisualStudio.com。 如果系统提示，请加入免费[Visual Studio Dev Essentials](https://visualstudio.microsoft.com/dev-essentials/)程序或使用 Visual Studio 订阅 id。 登录 在 Windows 服务器上，请参阅[取消阻止文件下载](../../debugger/remote-debugging-unblock-file-download.md)有关帮助下载的远程工具。|
    |Visual Studio 2013|[远程工具](https://msdn.microsoft.com/library/bt727f1t(v=vs.120).aspx#BKMK_Installing_the_Remote_Tools)|下载 Visual Studio 2013 文档中的页|
    |Visual Studio 2012|[远程工具](https://msdn.microsoft.com/library/bt727f1t(v=vs.110).aspx#BKMK_Installing_the_Remote_Tools)|下载 Visual Studio 2012 文档中的页|

2.  在下载页上，选择与你的操作系统 （x86、 x64、 ARM、 或 ARM64） 匹配的工具版本和下载远程工具。

    > [!IMPORTANT]
    >  我们建议为你的发布的 Visual Studio 安装远程工具的最新版本。 最新版本 (例如，15.8) 适用于早期版本 (例如，15.0);但是，早期版本不是与更高版本兼容的。 此外，必须安装具有相同的体系结构作为你想要将其安装操作系统的远程工具。 换而言之，如果你想要调试远程计算机运行 64 位操作系统上的 32 位应用程序，您必须在远程计算机上安装远程工具的 64 位版本。
    >
    >  对于 Windows 10 上调试 ARM 设备上，选择远程工具的最新版本可用的 ARM64 下载。  对于 Windows RT 的设备，选择选项仅适用于 Visual Studio 2015 RTW 下载的 ARM 版本。

3.  完成下载可执行文件后，转到下一节，并按照安装说明进行操作。

如果你尝试将远程调试器 (msvsmon.exe) 复制到远程计算机并运行它，请注意，**远程调试器配置向导**(**rdbgwiz.exe**) 仅在你下载时，才安装工具。 您可能需要使用该向导进行配置更高版本，尤其是如果你想将远程调试器作为服务运行。 有关详细信息，请参阅[（可选） 配置远程调试器作为服务](../../debugger/remote-debugging.md#bkmk_configureService)。
