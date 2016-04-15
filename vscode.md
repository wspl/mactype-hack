#VSCode
All versions are supported.

##Enable MacType

**Launching your VSCode with argument `--disable-direct-write`.**

You can do that via modifing shortcut property:

(You can find the shortcut on `C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Visual Studio Code`)

![](https://raw.githubusercontent.com/wspl/mactype-hack/master/vscode/vscode-shortcut.png)


##Fix Blurry on HiDPI

Append a launch argument: `--force-device-scale-factor=1`.

Append a item to "User Settings" (config.json) of VSCode: `"window.zoomLevel": 1.5`, You can modify `1.5` to the value of your desktop zoom scale.

![](https://raw.githubusercontent.com/wspl/mactype-hack/master/vscode/vscode-shortcut-hidpi.png)
![](https://raw.githubusercontent.com/wspl/mactype-hack/master/vscode/vscode-setting.png)
