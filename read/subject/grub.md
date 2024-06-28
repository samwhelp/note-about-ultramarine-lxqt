---
title: GRUB
nav_order: 3060
has_children: false
---


# GRUB


## 主題

* [如何更改GRUB佈景主題](#如何更改grub佈景主題)
* [下載安裝](#下載安裝)
* [設定採用](#設定採用)
* [參考文件](#參考文件)
* [相關筆記](#相關筆記)




## 如何更改GRUB佈景主題

> 以下以「[grub-theme-glass-remix](https://samwhelp.github.io/grub-theme-glass-remix/)」這個「GRUB 佈景主題」為例。




## 下載安裝

``` sh

## 產生暫時資料夾
mkdir -p "./tmp"


## 下載
wget -c "https://github.com/samwhelp/grub-theme-glass-remix/archive/refs/heads/main.tar.gz" -O "./tmp/grub-theme-glass-remix-main.tar.gz"


## 解壓縮
tar xf "./tmp/grub-theme-glass-remix-main.tar.gz" -C "./tmp"


## 確保有「/boot/grub2/themes」這個「資料夾」
sudo mkdir -p "/boot/grub2/themes"


## 將剛剛解開的「佈景主題」，安裝到「/boot/grub2/themes/grub-theme-glass-remix」這個路徑。
sudo cp -rf "./tmp/grub-theme-glass-remix-main/." "/boot/grub2/themes/grub-theme-glass-remix"

```

> 以上的步驟，就已經將「GRUB 佈景主題」安裝完成了。

> 接著要執行「設定採用」的步驟。




## 設定採用

可以編輯「`/etc/default/grub`」這個檔案，

原本的內容如下

``` sh
GRUB_TIMEOUT=5
GRUB_DISTRIBUTOR="$(sed 's, release .*$,,g' /etc/system-release)"
GRUB_DEFAULT=saved
GRUB_DISABLE_SUBMENU=true
GRUB_TERMINAL_OUTPUT="console"
GRUB_CMDLINE_LINUX="rhgb quiet"
GRUB_DISABLE_RECOVERY="true"
GRUB_ENABLE_BLSCFG=true
```

其中原本有一行如下

``` sh
GRUB_TERMINAL_OUTPUT="console"
```

將該行註解，改成如下

``` sh
#GRUB_TERMINAL_OUTPUT="console"
```

接著加入下面一行，指定要採用的「GRUB 佈景主題」。

``` sh
GRUB_THEME='/boot/grub2/themes/grub-theme-glass-remix/theme.txt'
```


> 上面的步驟完成後，接著一定要執行下面的步驟，

執行下面的指令，重新產生「`/boot/grub2/grub.cfg`」這個檔案。

``` sh
sudo grub-mkconfig -o /boot/grub2/grub.cfg
```

接著重新開機，就可以看到效果了。




## 更多的佈景主題

> 其他更多的「[GRUB 佈景主題](https://samwhelp.github.io/note-about-grub/read/theme.html)」。




## 參考文件

| GRUB Manual |
| ----------- |
| [Simple configuration handling](https://www.gnu.org/software/grub/manual/grub/html_node/Simple-configuration.html) |
| [Invoking grub-mkconfig](https://www.gnu.org/software/grub/manual/grub/html_node/Invoking-grub_002dmkconfig.html#Invoking-grub_002dmkconfig) |
| [Theme file format](https://www.gnu.org/software/grub/manual/grub/html_node/Theme-file-format.html) |


| Fedora Docs |
| ----------- |
| [The GRUB2 Bootloader – Installation and Configuration](https://docs.fedoraproject.org/en-US/quick-docs/grub2-bootloader/) |
| [Working with the GRUB 2 Boot Loader](https://docs.fedoraproject.org/en-US/fedora/latest/system-administrators-guide/kernel-module-driver-configuration/Working_with_the_GRUB_2_Boot_Loader/) |
| Wiki / [GRUB 2](https://fedoraproject.org/wiki/GRUB_2) |




## 相關筆記

| Link | GitHub |
| ---- | ------ |
| [GRUB 探索筆記](https://samwhelp.github.io/note-about-grub/) / [Use Theme](https://samwhelp.github.io/note-about-grub/read/howto/use_theme.html) | [GitHub](https://github.com/samwhelp/note-about-grub) |
