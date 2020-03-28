# homebrew-backup

备份homebrew安装的情况

## backup备份

```brew bundle dump --describe --force --file="./brewfile"```

备份好的文件将会存储到```./brewfile```文件中

## restore恢复

```/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```

首先安装homebrew

```brew bundle --file="./brewfile"```

根据备份文件，批量安装

## 其他

mas管理的App Store软件也可以用这样的方式备份和恢复，但是最好在安装好homebrew后安装mas，然后进行备份恢复。

```brew install mas```
