#Windows 10 Insider Preview
Latest supported version / 最后支持的版本： 最新的预览版 / 一周年版本

##Solution/解决方案

在更新到最新的 Win10 预览版以及某些早期版本之前，请务必禁用或者关闭 MacType 的「注册表模式」以及「随着开机启动」，否则更新后将无法正常进入系统，例如出现蓝屏、资源管理器不断崩溃重启等。

**原因：**MacType 使用了一个叫做 [EasyHook](http://easyhook.github.io/index.html) 的库，但是由于版本太旧，导致无法兼容新版 Windows 10 预览版。

**操作步骤：**

下载最新版的 EasyHook，标题类似 `EasyHook 2.x.xxxx Binaries .NET 3.5/4.0 (zip)`

下载地址：[http://easyhook.github.io/downloads.html](http://easyhook.github.io/downloads.html)


解压缩，推荐使用压缩包中 NetFX4.0 文件夹中的版本，按照以下方式重命名两个文件，并单独将这两个文件覆盖到 MacType 根目录：

`EasyHook32.dll` → `EasyHK32.dll`

`EasyHook64.dll` → `EasyHK64.dll`

至此，MacType 应该就可以正常工作了。经测试，可以支持「注册表兼容模式」以及「独立托盘模式」。
