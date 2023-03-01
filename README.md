# 模组开拓者汉化版

fork 自 https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder

### [![Download zip](https://custom-icon-badges.herokuapp.com/badge/-Download-blue?style=for-the-badge&logo=download&logoColor=white "Download zip")](https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder/releases/latest/download/ModFinder.zip)原版下载地址

### [![Download](https://custom-icon-badges.herokuapp.com/badge/-Download-blue?style=for-the-badge&logo=download&logoColor=white "Download zip")](https://github.com/magicskysword/ModFinder_CN/releases/latest/download/ModFinder.zip)汉化版下载地址

浏览与查看开拓者：正义之怒游戏Mod，及管理Mod依赖的工具

![截图](https://github.com/magicskysword/ModFinder_CN/blob/main/screenshots/main.png)

## 特点

* 浏览托管在Github和Nexus上的Mod
* 检测过期Mod
* 自动安装Github上的托管Mod
* 启用/禁用Mod
* 检测到缺少的依赖时，一键安装（Github）或弹出下载链接（Nexus）
* 卸载Mod
* 回滚Mod更新
* 以及更多

## 用户指南

下载最新版本，解压文件，运行 `ModFinder.exe`!

### **你需要安装 [.NET 桌面运行时 5.0](https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-desktop-5.0.0-windows-x64-installer) 或更高版本。**

### 你必须已经安装了 [UnityModManager](https://www.nexusmods.com/site/mods/21)。

### 如果依然无法正常使用，请查看 [故障排除](#故障排除)。

提示:

* 默认按Mod名和作者名进行搜索
* 你可以搜索具体名称、作者或[标签](https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder/blob/main/ModFinderClient/Mod/Tag.cs):
  * `a:bub` 搜索作者名包含“bub”的Mod，或使用 `-a:bub` 来排除它们
  * `n:super` 搜索Mod名包含“super”的Mod，或使用 `-n:super` 来排除它们
  * `t:game` 搜索标签包含“game”的Mod，或使用 `-t:game` 来排除它们
* 版本更新每30分钟检查一次，但你需要重启软件以获取更新
  * 提示：有时最新版本是为最新的游戏版本构建的（如测试版），请谨慎更新
* 当你打开软件时，缺少前置的Mod会优先展示，其次是已安装的Mod
* 溢出菜单有更多的功能，如查看变更日志、描述和主页
* 当您使用ModFinder更新一个mod时，您可以恢复到以前的版本，打开溢出菜单并选择“回滚”

### 缺少Mod?

请通知开发者往源项目提 [issue](https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder/issues/new)。（非本项目）

## 开发者指南

请参考源项目：https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder

## 故障排除

* 请确保你已经安装了 [UnityModManager](https://www.nexusmods.com/site/mods/21)
  * 运行管理器并为正义之怒初始化
* 请确保你安装了 [.NET 桌面运行时 5.0](https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-desktop-5.0.0-windows-x64-installer) 或更高版本
  * .NET 6.0 与 .NET 7.0 应该也能使用，如果不行，请使用上面的链接安装5.0版本
  * .NET 5.0与 .NET 运行时 5、 .NET 桌面运行时 5.0不是一样东西；如果你认为你已经安装了.net，但是依然无法运行，请尝试从上述链接进行安装
* 尝试 [以管理员身份运行](https://www.itechtics.com/run-programs-administrator/)
* 确保没有被杀毒软件拦截
  * 一些杀毒软件会标记为木马软件
    * ModFinder向GitHub发送下载mod元数据和mod本身的请求
    * ModFinder也写入文件(日志)和删除，移动和解压缩文件相关的mods
  * 更新日志包括一个sha1散列，您可以使用它来验证您的下载（注：翻译版本并未包含此hash值）
  * 下面是v1.1 on的扫描结果： [VirusTotal](https://www.virustotal.com/gui/file/882b5b1e5eb0dc2d51413a663d116b89856ab3f35681505e7d5286f1ecd0aee6/detection) （注：这是源mod的扫描结果）
* 提交 [问题](https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder/issues/new) 或在Discord上寻求帮助
  * 分享你的日志文件: `%UserProfile%\AppData\Local\Modfinder\Log.txt`

### 对某个Mod有问题?

如果对安装、下载、显示信息或任何其他内容有疑问，可以提交[问题](https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder/issues/new)，这包含不能使用或已废弃的Mod。

（注：这是对源Mod提交的问题，有关汉化问题请在本Mod下提交）

### 其他问题?

没错：提交[问题](https://github.com/Pathfinder-WOTR-Modding-Community/ModFinder/issues/new). 并包含你的日志内容： `%UserProfile%\AppData\Local\Modfinder\Log.txt`.

## 致谢

该部分内容保持原汁原味（故意的）

* Barley for starting this project in the first place ([ModFinder_WOTR](https://github.com/BarleyFlour/ModFinder_WOTR)) and working with Bubbles to complete like 80% before I decided to finish it
* Bubbles for his excellent work on the UI styling and Barley for handling the GitHub action setup
* The modding community on [Discord](https://discord.com/invite/owlcat), an invaluable and supportive resource for help modding.
* All the Owlcat modders who came before me, wrote documents, and open sourced their code.

## 对Mod开发感兴趣？

* 查看 [OwlcatModdingWiki](https://github.com/WittleWolfie/OwlcatModdingWiki/wiki).
* 加入 [Discord](https://discord.com/invite/owlcat).
