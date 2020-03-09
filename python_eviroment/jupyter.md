# 1. jupyter



## 1.1. 卸载pip安装的jupyter

安装pip-autoremove
`pip install pip-autoremove --user`
注意：mac无法安装，可以加--user

删除jupyter和依赖包
`pip-autoremove jupyter`




## 1.2. 启动python2.7下的jupyter

输入jupyter notebook 无法启动。是系统中文编码引起的问题，用以下方法可以启动
`LANG=zn jupyter-notebook`