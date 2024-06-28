---
title: 語系
nav_order: 3010
has_children: false
---


# 語系


## 主題

* [相關議題](#相關議題)
* [Docs](#docs)
* [設定檔路徑](#設定檔路徑)
* [相關指令](#相關指令)
* [Package](#package)




## 相關議題

| 相關議題 |
| --- |
| [字型](https://samwhelp.github.io/note-about-ultramarine-lxqt/read/subject/font.html) |
| [輸入法](https://samwhelp.github.io/note-about-ultramarine-lxqt/read/subject/input-method.html) |




## Docs

* Fedora Docs / [System Locale and Keyboard Configuration](https://docs.fedoraproject.org/en-US/fedora/latest/system-administrators-guide/basic-system-configuration/System_Locale_and_Keyboard_Configuration/)




## 設定檔路徑

| 設定檔路徑 |
| /etc/locale.conf |

執行

``` sh
cat /etc/locale.conf
```

顯示

```
LANG="en_US.UTF-8"
```




## 相關指令

執行

``` sh
locale
```

顯示

```
LANG=en_US.utf8
LC_CTYPE="en_US.utf8"
LC_NUMERIC="en_US.utf8"
LC_TIME="en_US.utf8"
LC_COLLATE="en_US.utf8"
LC_MONETARY="en_US.utf8"
LC_MESSAGES="en_US.utf8"
LC_PAPER="en_US.utf8"
LC_NAME="en_US.utf8"
LC_ADDRESS="en_US.utf8"
LC_TELEPHONE="en_US.utf8"
LC_MEASUREMENT="en_US.utf8"
LC_IDENTIFICATION="en_US.utf8"
LC_ALL=
```

執行

``` sh
localectl status
```

顯示

```
System Locale: LANG=en_US.UTF-8
    VC Keymap: us
   X11 Layout: us
    X11 Model: pc105
```




執行

``` sh
locale -a | grep zh
```

顯示

```
lzh_TW
lzh_TW.utf8
zh_CN
zh_CN.gb18030
zh_CN.gb2312
zh_CN.gbk
zh_CN.utf8
zh_HK
zh_HK.big5hkscs
zh_HK.utf8
zh_SG
zh_SG.gb2312
zh_SG.gbk
zh_SG.utf8
zh_TW
zh_TW.big5
zh_TW.euctw
zh_TW.utf8
```



執行

``` sh
localectl list-locales | grep zh
```

顯示

```
lzh_TW.UTF-8
zh_CN.UTF-8
zh_HK.UTF-8
zh_SG.UTF-8
zh_TW.UTF-8
```


執行

``` sh
sudo localectl set-locale LANG="zh_TW.UTF-8"
```

執行

``` sh
cat /etc/locale.conf
```

顯示

```
LANG=zh_TW.UTF-8
```


執行

``` sh
sudo localectl set-locale LANG="en_US.UTF-8"
```




## Package

* [glibc-all-langpacks](https://packages.fedoraproject.org/pkgs/glibc/glibc-all-langpacks/)
