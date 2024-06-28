---
title: 如何安裝「嘸蝦米輸入法」
nav_order: 3201
has_children: false
parent: fcitx5
grand_parent: 輸入法
---


# 如何安裝「嘸蝦米輸入法」

> 如何安裝「[fcitx5-table-extra](https://packages.fedoraproject.org/pkgs/fcitx5-table-extra/fcitx5-table-extra)」。




## 主題

* [微調腳本](#微調腳本)
* [指令安裝](#指令安裝)
* [切換輸入法架構](#切換輸入法架構)
* [加入輸入法](#加入輸入法)
* [備註](#備註)




## 微調腳本

| 微調腳本 | 中文輸入法 |
| -------- | ---------- |
| [fcitx5-table-boshiamy 安裝設定腳本](https://github.com/samwhelp/ultramarine-lxqt-adjustment/tree/main/prototype/main/im-config/fcitx5/fcitx5-table-boshiamy) | 嘸蝦米輸入法 |




## 指令安裝

執行下面指令，安裝「imsettings」。

``` sh
sudo dnf install imsettings
```

執行下面指令，安裝「fcitx5」。

``` sh
sudo dnf install fcitx5
```

執行下面指令，安裝「[fcitx5-table-extra](https://packages.fedoraproject.org/pkgs/fcitx5-table-extra/fcitx5-table-extra)」和「[fcitx5-chinese-addons](https://packages.ubuntu.com/noble/fcitx5-chinese-addons)」。

``` sh
sudo dnf install fcitx5-table-extra fcitx5-chinese-addons
```

執行下面指令，確保安裝支援「GTK」和「QT」環境所需要的「Package」。

``` sh
sudo dnf install fcitx5-gtk2 fcitx5-gtk3 fcitx5-gtk4 fcitx5-qt fcitx5-qt6
```

執行下面指令，安裝「圖形設定介面」的「輔助工具」。

``` sh
sudo dnf install fcitx5-configtool
```

> 可以參考我的「[package-list.txt](https://github.com/samwhelp/ultramarine-lxqt-adjustment/blob/main/prototype/main/im-config/fcitx5/fcitx5-chewing/package-list.txt)」。

| Package |
| ------- |
| [imsettings](https://packages.fedoraproject.org/pkgs/imsettings/imsettings) |
| [fcitx5](https://packages.fedoraproject.org/pkgs/fcitx5/fcitx5) |
| [fcitx5-table-extra](https://packages.fedoraproject.org/pkgs/fcitx5-chinese-addons/fcitx5-table-extra) |
| [fcitx5-chinese-addons](https://packages.fedoraproject.org/pkgs/fcitx5-chinese-addons/fcitx5-chinese-addons) |
| [fcitx5-configtool](https://packages.fedoraproject.org/pkgs/fcitx5-configtool/fcitx5-configtool) |
| [fcitx5-gtk2](https://packages.fedoraproject.org/pkgs/fcitx5-gtk2/fcitx5-gtk2) |
| [fcitx5-gtk3](https://packages.fedoraproject.org/pkgs/fcitx5-gtk3/fcitx5-gtk3) |
| [fcitx5-gtk4](https://packages.fedoraproject.org/pkgs/fcitx5-gtk4/fcitx5-gtk4) |
| [fcitx5-qt](https://packages.fedoraproject.org/pkgs/fcitx5-qt/fcitx5-qt) |
| [fcitx5-qt6](https://packages.fedoraproject.org/pkgs/fcitx5-qt6/fcitx5-qt6) |


> 上面的安裝指令，可以合併在一起如下

``` sh
sudo dnf install \
	imsettings \
	fcitx5 \
	fcitx5-table-extra \
	fcitx5-chinese-addons \
	fcitx5-gtk2 \
	fcitx5-gtk3 \
	fcitx5-gtk4 \
	fcitx5-qt \
	fcitx5-qt6 \
	fcitx5-configtool

```




## 切換輸入法架構

> 執行下面指令，顯示有那些「輸入法架構」可供選擇。

``` sh
imsettings-list
```

顯示

```
* 1: IBus[ibus.conf] (recommended)
  2: X compose table[xcompose.conf]
  3: fcitx5[fcitx5.conf]
```

> 執行下面指令，將「輸入法架構」切換到「fcitx5」。

``` sh
imsettings-switch fcitx5
```

> 重新登出，然後登入，就會生效




## 加入輸入法

透過「圖形操作介面程式(`fcitx5-configtool`)」，

加入「嘸蝦米輸入法(`fcitx5-table-boshiamy`)」這個「輸入法」。




## 備註

### ~/.config/imsettings/xinputrc

上面的步驟「`imsettings-switch fcitx5`」，會產生「`~/.config/imsettings/xinputrc`」這個檔案。

執行

``` sh
file ~/.config/imsettings/xinputrc
```

顯示

```
/home/user/.config/imsettings/xinputrc: symbolic link to /etc/X11/xinit/xinput.d/fcitx5.conf
```

> 表示「`~/.config/imsettings/xinputrc`」這個檔案，會軟連結到「/etc/X11/xinit/xinput.d/fcitx5.conf」這個檔案。


執行下面指令，觀看「`~/.config/imsettings/xinputrc`」這個檔案的內容

``` sh
cat ~/.config/imsettings/xinputrc
```

顯示

```
XIM=fcitx5
XIM_PROGRAM=/usr/bin/fcitx5
ICON="fcitx5"
XIM_ARGS="-D"
PREFERENCE_PROGRAM=/usr/bin/fcitx5-configtool
SHORT_DESC="fcitx5"
GTK_IM_MODULE=fcitx
if test -f /usr/lib/qt4/plugins/inputmethods/qtim-fcitx5.so || \
   test -f /usr/lib64/qt4/plugins/inputmethods/qtim-fcitx5.so || \
   test -f /usr/lib/qt5/plugins/platforminputcontexts/libfcitx5platforminputcontextplugin.so || \
   test -f /usr/lib64/qt5/plugins/platforminputcontexts/libfcitx5platforminputcontextplugin.so;
then
    QT_IM_MODULE=fcitx
else
    QT_IM_MODULE=xim
fi

# workaround for gnome users
if [ "$XDG_SESSION_DESKTOP" = "gnome"  ]; then
    /usr/bin/systemd-run --user --unit=$XIM $XIM_PROGRAM $XIM_ARGS
fi

```




## 相關議題

| 相關議題 |
| --- |
| [如何簡易安裝「fcitx5-table-boshiamy」](https://samwhelp.github.io/note-about-ubuntu/read/subject/im/fcitx5/howto/install-fcitx5-table-boshiamy.html) |
