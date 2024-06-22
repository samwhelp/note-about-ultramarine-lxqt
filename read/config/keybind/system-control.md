---
title: 系統操作
nav_order: 5001
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 系統操作


## 重新載入設定

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/SystemExit.php#L3-L6)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + Shift + c`  | 重新載入設定 | `Reconfigure` (openbox 內建) |




## 登出

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/SystemExit.php#L11-L30)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + Shift + x`  | 顯示登出確認對話框 | `lxqt-leave --logout` |
| `Alt + Ctrl + x`  | 示登出確認對話框 (Openbox) | `Exit` (openbox 內建) |




## 離開

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/SystemExit.php#L44-L65)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + Shift + z`  | 顯示離開選單 | `lxqt-leave` |
| `Alt + Ctrl + z`  | 顯示鎖定螢幕確認對話框 | `lxqt-leave --lockscreen` |




## 切換「顯示桌面」

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/SystemToggleShowDesktop.php#L3-L5)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Win + d`  | 顯示「桌面操作選單」 | `ToggleShowDesktop` (openbox 內建) |

> 也可以在「桌面」使用「滑鼠左鍵」，反覆按下，就會切換「顯示桌面」。

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Mousebind/Root.php#L5-L8)
