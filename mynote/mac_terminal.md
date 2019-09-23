# mac terminal command

- clean the Trash

```
sudo rm -rf ~/.Trash/
```

- check the volume

```bash
df -h            #命令查看整个硬盘的大小 ，-h表示人可读的
du -d 1 -h    #命令查看当前目录下所有文件夹的大小 -d 指深度，后面加一个数值
```
- find file
```bash
find path -name
find path -size +100M
```

- set the alias

```bash
alias emacs='/Applications/Emacs.app/Contents/MacOS/Emacs'
```

- ls 分页显示
```bash
ls -al |more
```

挂载网盘

        EXAMPLES
     This example shows the proper url to use to mount the share PUBLIC from
     the SMB server myserver :

           mkdir /smb/public
           mount -t smbfs //username:userpass@myserver/PUBLIC /smb/public

     This example shows the proper url to use to mount the share PUBLIC from
     the SMB server myserver as guest:

           mkdir /smb/public
           mount -t smbfs //guest:@myserver/PUBLIC /smb/public
     Note: You should always use the system mount command and never call
     mount_smbfs directly.