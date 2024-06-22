---
title: 工作空間切換
nav_order: 5040
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 工作空間切換


## 我個人定義的個工作空間

| 工作空間 | 名稱  |
| -------- | ----- |
| 1        | File  |
| 2        | Edit  |
| 3        | Web   |
| 4        | Term  |
| 5        | Misc  |


## 指定切換

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WorkspaceSwitch.php#L80)

| 按鍵組合  | 功能                    | 執行指令                       |
| --------- | ----------------------- | ------------------------------ |
| `Alt + Ctrl + 1` | 切換到工作空間 1 (File) | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 2` | 切換到工作空間 2 (Edit) | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 3` | 切換到工作空間 3 (Web)  | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 4` | 切換到工作空間 4 (Term) | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 5` | 切換到工作空間 5 (Misc) | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 6` | 切換到工作空間 1        | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 7` | 切換到工作空間 2        | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 8` | 切換到工作空間 3        | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 9` | 切換到工作空間 4        | `GoToDesktop` (openbox 內建) |
| `Alt + Ctrl + 0` | 切換到工作空間 5        | `GoToDesktop` (openbox 內建) |

## 循環切換

* [設定片段](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/lxqt-config/Main/asset/overlay/etc/skel/.config/openbox/helper/share/gen/openbox-gen-rc/Section/Keybind/WorkspaceSwitch.php#L8-L18)


| 按鍵組合  | 功能                 | 執行指令                   |
| --------- | -------------------- | -------------------------- |
| `Alt + a` | 切換到上一個工作空間 | `GoToDesktop` (openbox 內建) |
| `Alt + s` | 切換到下一個工作空間 | `GoToDesktop` (openbox 內建) |


> 也可以在「桌面」，使用「滑鼠中鍵」，上下滾動，切換「工作空間」。

> 也可以在「Panel」的「Workspace區」，使用「滑鼠中鍵」，上下滾動，切換「工作空間」。
