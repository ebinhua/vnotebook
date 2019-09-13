# sublime

- 命令行启动sublime  

使用软连接（可以理解为快捷方式）将Sublime提供的命令行工具直接连接到/usr/local/bin/这个路径下。  
将/usr/local/bin/subl连接到Mac下的sublime应用提供的命令行工具subl。

```bash
n -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```


- 配置语法高亮  

```bash
1. 点击右下角的语法高亮选项菜单
2. 在菜单的顶部Open all with current extension as…子菜单中，改成Matlab
```