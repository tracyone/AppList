# Mac OS X Software Install Guide

## keepass

下载[keepass for mac](http://keepass.info/download.html)

keepass是.net程序，所以在mas和linux下要运行必须运行.net framework兼容的mono，点我下载[mono for mac](http://www.mono-project.com/download/#download-mac)

ubuntu 下安装可通过ppa安装即可

```bash

```

## coreutils

```bash
brew install coreutils
```
装完之后shell的配置文件中设置`PATH`变量

```bash
PATH="/usr/local/opt/coreutils/libexec/gnubin:/usr/local/bin:$PATH"
```

第一个路径是coreutils的可执行程序的路径，第二个是brew安装其它程序默认的可执行程序路径，我们都将它放在前面，保证我们使用的时这些程序，而非系统自带。

上面的coreutils只是包含有限的核心程序而已，还有好多经常使用的没有...所以我们还要装下面的:

```bash
brew install binutils
brew install diffutils
brew install ed --default-names
brew install findutils --with-default-names
brew install gawk
brew install gnu-indent --with-default-names
brew install gnu-sed --with-default-names
brew install gnu-tar --with-default-names
brew install gnu-which --with-default-names
brew install gnutls
brew install grep --with-default-names
brew install gzip
brew install screen
brew install watch
brew install wdiff --with-gettext
brew install wget
brew install gpatch
brew install m4
brew install make
brew install git
brew install less
```

## brew相关




