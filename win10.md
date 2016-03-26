#Windows 10 Insider Preview
Latest supported version / 最后支持的版本： 14291

##Solution/解决方案

在更新 14291 之前，请务必将 MacType 的注册表模式以及开机启动禁用，否则更新后可能无法正常进入系统，例如出现蓝屏。

原因是 MacType 使用了一个叫做 [EasyHook](http://easyhook.github.io/index.html) 的库，但是由于版本太旧，导致无法兼容新版 Windows 10 预览版。

解决方案就是下载最新版的 EasyHook，标题类似 `EasyHook 2.x.xxxx Binaries .NET 3.5/4.0 (zip)`

下载地址：[http://easyhook.github.io/downloads.html](http://easyhook.github.io/downloads.html)


解压缩，推荐使用压缩包中 NetFX4.0 文件夹中的版本，按照以下方式重命名两个文件，并单独将这两个文件覆盖到 MacType 根目录：

`EasyHook32.dll` -> `EasyHK32.dll`

`EasyHook64.dll` -> `EasyHK64.dll`

自此，MacType 应该就可以正常工作了。
