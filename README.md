# MacType-Hack
为那些默认不支持 MacType 的应用程序或操作系统提供字体渲染兼容方案。

Solutions for applying MacType to not supported programs/os.

## 面向独显用户的终极字体美化技巧
解决方案：开启 “超虚拟分辨率” 功能，基本所有 14 年后推出的新显卡都支持，Nvidia 显卡叫做 DSR，AMD 显卡叫做 VSR。

例如我目前正在使用 2560*1440 分辨率的显示器，GTX1080 作为输出显卡。
1. 在 Nvidia 控制面板开启 2.25x 的 DSR 缩放
2. 同样的位置，DSR 平滑度设置为 30%。（这个参数可以细微调整到你最喜欢的效果）
3. 将系统分辨率修改为开启 DSR 后的分辨率，例如我这里是 3840*2180
4. 将缩放与布局设置为 200% 以上

然后你就能获得极佳的 Windows 字体抗锯齿体验了！

（AMD 显卡似乎效果不是很好，希望得到反馈）

## 【MacType 重要更新】

最新的 MacType 已经内置 Direct-Write 应用程序渲染方案：

下载地址：[https://github.com/snowie2000/mactype/releases](https://github.com/snowie2000/mactype/releases)

官方网站：[http://www.mactype.net/](http://www.mactype.net/)



若需要开启 Direct-Write 渲染需要在配置文件中添加 `DirectWrite=1` 以启用。

**若曾经使用过 MacType-Patch 的用户请删除曾经添加的两个 EasyHook DLL 文件。**



（感慨一下，MacType 终于重新开始维护了，连官方网站都有了）

## Solutions / 解决方案

* **Programs / 程序**

  * [*Chromium](chromium.md)
  * [Firefox](firefox.md)
  * [Microsoft Visual Studio 2010+](https://www.textarea.com/simodorg/solve-mactype-doesnt-work-in-visual-studio-2015-251/)
  * [Microsoft Visual Studio Code](vscode.md)
  * [Github Atom](atom.md)
  * [Universal Windows Application (Experimental/不建议使用)](http://tieba.baidu.com/p/4040192792)
  * [JetBrains Series: Intellij IDEA, Android Studio, PHPStorm, PyCharm etc.](jetbrains.md)


* **Operating Systems / 操作系统**

  * [Windows 10 Insider Preview](win10.md)

## Contributors / 贡献者

* [Plutonist (wspl)](https://github.com/wspl)
* [Wowse](https://github.com/wowse)
* [foisonocean](https://github.com/foisonocean)
