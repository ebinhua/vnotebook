
## mac 安装使用aria2

### 1.mac install aria2

https://yalv.me/aria2/

### 2.aria2 web 控制台

aria2c.com
http://aria2.me/webui-aria2/

### 3.关闭生成与文件同名的的.aria2后缀文件

在~/.aria2/aria2.conf配置文件下面，加上一条命令  
`on-download-complete="rm -f "$3.aria2"`
并将force-save更改  
`force-save=false`
然后重启 aria2 
`aria2c restart`
如果还存在该问题，重启电脑即可。



## 路由器安装和使用aria2

### 1. 刷梅林固件

https://koolshare.cn/portal.php
ebinhua
Island12

https://koolshare.cn/thread-139322-1-1.html
http://firmware.koolshare.cn


### 2.aria2 router download 115 setting
https://koolshare.cn/thread-30944-1-1.html
http://koolshare.cn/thread-125218-1-1.html

### 3. chrome 115插件

#### chrome 11115插件下载
https://github.com/acgotaku/115/commits/master

### 4.插件115设置aria2主机
http://token:12345678@192.168.50.1:6800/jsonrpc

### 5.虚拟内存minitool downlod
http://www.xdowns.com/soft/6/7/2013/Soft_102850.html

### 115 http respones bad
enable-http-pipelining=false

