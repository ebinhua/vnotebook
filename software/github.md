# github


link http://github.com/ebinhua

## user information
user: ebinhua
password: Island#1234
email:13928849498@139.com

## configure username and email

`git config --global uesr.name "ebinhua"`
`git config --global user.eamil "13928849498@139.com"`


## 配置git in mac

link [configure git in mac](https://www.cnblogs.com/puqunzhu/p/9774269.html)

1、设置username和email（github每次commit都会记录他们）
`git config --global uesr.name "ebinhua"`
`git config --global user.eamil "13928849498@139.com"`

2、通过终端命令创建ssh key

`ssh-keygen -t rsa -C "13928849498@139.com"` 回车会有以下输出

```bash
qunzhudeMacBook-Air:git qunzhupu$ ssh-keygen -t rsa -C "13928849498@139.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/qunzhupu/.ssh/id_rsa): 
/Users/qunzhupu/.ssh/id_rsa already exists.
Overwrite (y/n)? n
```
由于这里我原来已经创建过，这里我选n，没有创建过的，会要求确认路径和输入密码，我们这使用默认的一路回车就行。成功的话会在~/下生成.ssh文件夹，进去，打开id_rsa.pub，复制里面的key。

3、终端查看.ssh/id_rsa.pub文件:

`open .ssh/id_rsa.pub`回车后，就会新弹出一个终端，然后复制里面的key。
或者用cat命令查看`cat .ssh/id_rsa.pub`

4、登录GitHub（默认你已经注册了GitHub账号），添加ssh key，点击Settings,点击New SSH key,添加key

5、链接验证 `ssh -T git@github.com` 终端输出结果


## please tell me who you are
提示也就是需要你登录一下，确认你的身份，但是不要按照其提示输入，
先输入命令`git config user.name “username"`
换行输入`git config user.email “email”`
输入正确的之后就能使用 git add 、commit等命令进行版本控制了
