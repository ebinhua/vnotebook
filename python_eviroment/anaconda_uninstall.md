# MAC删除anaconda

### 第一步，删除Anaconda的配置，命令如下：

 `conda install anaconda-clean`  : 安装anaconda-clean
 `anaconda-clean`: 执行anaconda-clean
 `rm -r /Users/zc/.anaconda_backup/2019-*`: 删除备份文件

  运行完第二个命令，命令行会提示是否删除，直接选y就可以，并且会在你的根目录下会生成一个备份
  第三个命令中备份文件名需要更改为自己的备份名字

### 第二步，删除Anaconda的文件夹，命令如下：

`rm -rf ~/Apps/anaconda3`
  注：文件夹可能在其他位置，请确认


### 第三步，删除 ~/.bash_profile中anaconda的环境变量，可以使用vim打开删除

`vim ~/.bash_profile`

### 第四步，删除Anaconda的可能存在隐藏的文件，建议执行一下命令：

`rm -rf ~/.condarc ~/.conda ~/.continuum`

经过上述4步后，Anaconda被彻底删除了。

