---
title: 系統選單
nav_order: 5002
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 系統選單


## 顯示「視窗操作選單」

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/MenuClient.php#L3-L7)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + Space`  | 顯示「視窗操作選單」 | `client-menu` (openbox 內建) |

> 也可以在「視窗標題列」使用「滑鼠右鍵」，就會顯示「視窗操作選單」。




## 顯示「Runner 對話框 (Lxqt)」

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L15-L18)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + F2`  | 顯示「Runner 對話框」 | `path=/runner/show_hide_dialog` (Lxqt) |




## 顯示「主要功能選單 (Lxqt)」

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/blob/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/lxqt/globalkeyshortcuts.conf#L10-L13)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Alt + F1`  | 顯示「主要功能選單」 | `path=/panel/mainmenu/show_hide` (Lxqt) |



## 顯示「主要功能選單 (Openbox)」

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/MenuRoot.php)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Win + Space`  | 顯示「主要功能選單」 | `root-menu` (openbox 內建) |




## 顯示「工作空間操作選單」

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/MenuClientList.php)

| 按鍵組合           | 功能        | 執行指令             |
| ----------------- | ------------ | -------------------- |
| `Win + c`  | 顯示「工作空間操作選單」 | `client-list-combined-menu` (openbox 內建) |
| `Alt + F3`  | 顯示「工作空間操作選單」 | `client-list-combined-menu` (openbox 內建) |

