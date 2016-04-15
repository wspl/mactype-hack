# Visual Studio Code support for MacType

There are two ways for tweaking VS Code to work with MacType, both have their pros and cons.

## By changing code
**Works on 1.0.0**, from all CLI, shortcut and original exe.
Other versions might work too but it's not suggested to try as it would break the editor.

You can do this by replacing file `<VS Code Location>\resources\app\out\vs\workbench\electron-main\main.js` by [this one](https://raw.githubusercontent.com/wspl/mactype-hack/master/vscode/main.js)

where `<VS Code Location>` is the folder, where VS Code is installed.

Then kill all of your VS Code processes and start editor again.

---

## By adding flag `--disable-direct-write` to shortcut
Works on any VS Code version, **only if opened from shortcut**

You'll most likely find the shortcut in `C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Visual Studio Code`

Then modify shortcut properties so there is `--disable-direct-write` at the end:

![properties](https://raw.githubusercontent.com/wspl/mactype-hack/master/vscode/vscode-shortcut.png)

---

## Fix Blurry fonts on HiDPI
Append another argument: `--force-device-scale-factor=1`.

Also append config entry to "User Settings" (config.json) of VS Code: `"window.zoomLevel": 1.5`, You can modify `1.5` to the value of your desktop zoom scale.

![properties](https://raw.githubusercontent.com/wspl/mactype-hack/master/vscode/vscode-shortcut-hidpi.png)
![config.js](https://raw.githubusercontent.com/wspl/mactype-hack/master/vscode/vscode-setting.png)
