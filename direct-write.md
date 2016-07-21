# Direct-Write 解决方案

参考 / Reference：[http://silight.hatenablog.jp/entry/MacTypePatch](http://silight.hatenablog.jp/entry/MacTypePatch)

**(This is an untranslated version, welcome translation)**

## 简介
　　霓虹万能的民间程序员终于研究出了修复 Direct Write 渲染效果的黑科技，我在 Insider Preview Build.14393 上试用，表示效果很惊艳。其一是修正了糟糕的字体畸形问题，其二就是启用/增强了灰阶抗锯齿。

![放个截图让大家感受一下](https://cloud.githubusercontent.com/assets/2133311/17010686/c5a335d8-4f38-11e6-95db-cae19fa2e7d3.png)

　　实际上渲染效果和原生 MacType 还是有一定的差别的，它更加的细，更接近于 macOS / Unity 的渲染效果。


## 使用方法

1. 先到相关 Repo 获取最新的 Release：[https://github.com/silight-jp/MacType-Patch/releases](https://github.com/silight-jp/MacType-Patch/releases)

2. 解压后，将 `EasyHK32.dll` 和 `EasyHK64.dll` 还有 `win8.1 or later` 文件夹内的 `UserParams.ini` 全部拷贝到 MacType 的程序目录并覆盖同名文件

3. 重启 MacType，开启 Chromium 的 Direct-Write 渲染。

4. 若是没有效果，尝试将 `EasyHK32.dll` 复制到 `C:\Windows\System32` 下，将 `EasyHK64.dll` 复制到 `C:\Windows\SysWOW64` 下，重启 MacType，再尝试效果。

5. 如果上面所有操作都执行完后还是没有效果，尝试重启系统，或者修改兼容性相关选项。


## 存在问题

1. 不支持 Edge 以及其他 UWP 应用，具体原因不详，按照作者的建议使用注册表模式也没有效果。

2. 在 Office 2016 下没有效果 / 效果不佳
