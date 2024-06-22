---
title: 視窗基本操作
nav_order: 5020
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 視窗基本操作

* [關閉視窗](#關閉視窗)
* [全螢幕](#全螢幕)
* [最大化](#最大化)
* [最小化](#最小化)
* [開始視窗移動](#開始視窗移動)
* [開始視窗更改大小](#開始視窗更改大小)
* [取消開始相關操作](#取消開始相關操作)
* [永遠在最上方](#永遠在最上方)
* [內容區塊收合](#內容區塊收合)
* [切換顯示隱藏視窗裝飾](#切換顯示隱藏視窗裝飾)
* [將下方視窗移上來](#將下方視窗移上來)


## 關閉視窗

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowClose.php)

| 按鍵組合          | 功能     | 執行指令         |
| ----------------- | -------- | ---------------- |
| `Win + q`         | 關閉視窗 | `Close` (openbox 內建) |


## 全螢幕

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowToggleFullscreen.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + f` | 視窗全螢幕 | `ToggleFullscreen` (openbox 內建) |


## 最大化

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowToggleMaximize.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + w` | 最大化 | `ToggleMaximize` (openbox 內建) |

> 也可以在「標題列」，使用「滑鼠左鍵」，點選兩下，切換視窗最大化。

## 最小化

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowIconify.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + x` | 最小化 | `Iconify` (openbox 內建) |


## 開始視窗移動

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowBeginMove.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + e` | 開始視窗移動 | `Move` (openbox 內建) |

> 按「Escape」鍵，取消「開始視窗移動」。


## 開始視窗更改大小

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowBeginResize.php#L3)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + r` | 開始視窗更改大小 | `Resize` (openbox 內建) |

> 按「Escape」取消「開始視窗更改大小」。


## 永遠在最上方

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowToggleAlwaysOnTop.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + t` | 永遠在最上方 | `ToggleAlwaysOnTop` (openbox 內建) |


## 內容區塊收合

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowToggleShade.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + y` | 內容區塊收合 | `ToggleShade` (openbox 內建) |


> 也可以在「標題列」，使用「滑鼠中鍵」上下滾動，切換內容區塊收合。


## 切換顯示隱藏視窗裝飾

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowToggleDecorations.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + v` | 切換顯示隱藏視窗裝飾(Decorations) | `ToggleDecorations` (openbox 內建) |

> 視窗裝飾(Decorations)，最明顯的，就可以看到標題列隱藏或是顯示。

## 將下方視窗移上來

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WindowRaiseLower.php)

| 按鍵組合  | 功能       | 執行指令                      |
| --------- | ---------- | ----------------------------- |
| `Win + u` | 將下方視窗移上來 | `RaiseLower` (openbox 內建) |
