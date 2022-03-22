## Welcome to GitHub Pages

[![C](https://s4.ax1x.com/2021/12/29/TghaxP.jpg)](https://imgtu.com/i/TghaxP)



Git入门教程：

git在安装完成后会在鼠标右键菜单中添加“Git bash here”选项

![image-20220322221318836](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322221318836.png)

​	Git GUI Here使用的是图形界面，Git Bash Here使用的是命令行，这里用命令行做演示。

​	使用Git首先要有一个代码仓库，可以在Github或Gitee上创建（也可使用本地仓库），此处以Gitee上的仓库做演示。

![image-20220322222501397](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322222501397.png)

​	复制仓库的SSH地址：git@gitee.com:DtaoCN_admin/xiaoche.git

​	![image-20220322222630540](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322222630540.png)

在你要存放代码的地方右键鼠标，打开终端bash

![image-20220322222813553](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322222813553.png)

输入 git clone 加上仓库的地址： `git clone git@gitee.com:DtaoCN_admin/xiaoche.git`并回车

![image-20220322222913367](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322222913367.png)

代码仓库就会被克隆到你打开bsah终端的文件夹，此文件夹可以是桌面

![image-20220322223005928](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322223005928.png)

点进去就能看到仓库的所有代码。



下面介绍两种操作：git push 和 git pull

/..................git pull

在仓库根目录打开bash终端使用 `git pull`命令可以随时从gitee的仓库中同步最新的修改内容。

/.................git push:

我们对某段文件（以main.c为例）进行修改后

![image-20220322223310609](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322223310609.png)



![image-20220322223343905](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322223343905.png)

保存文件，已完成计划工作时，可将代码保存到gitee仓库：

1 ![image-20220322223937815](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322223937815.png)



进入到你克隆下的仓库里并打开bash，或在刚才打开bash的位置cd 进入下载的仓库根目录

2 ![image-20220322224016783](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322224016783.png)

终端里使用 `git add 加你修改的文件`，也可以直接 `git add *`将所有文件都放入暂存区。

3 使用 `git commit -m "加入你对修改的说明" ` 或直接 `git commit`

4 ![image-20220322224204892](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322224204892.png)

此时会进入一个文本编辑器，我设置的nano，但默认的是使用Vim

​	(1)vim : 按下i 进入编辑模式，移动方向键将光标移动到你修改的文件名前面

![image-20220322224403176](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322224403176.png)

​		删除你修改文件前的 # （有时改动的文件不止一个），然后按下esc进入vim的命令模式，输入wq 即可保存退出，稍后便commit完成了。

​	(2)nano: 直接使用方向键移动光标到修改文件前的 #位置，将其删除，按下 Ctrl 加 x, 再按Y回车确定即可保存退出。

![image-20220322224808664](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322224808664.png)

![image-20220322224850199](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322224850199.png)



5 当commit结束后，就可以使用 `git push` 将你的修改推送到gitee仓库

![image-20220322225339222](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322225339222.png)

之后别人使用git clone或者git pull命令同步的代码都将会有你修改的内容

![image-20220322225501328](C:\Users\Dtao\AppData\Roaming\Typora\typora-user-images\image-20220322225501328.png)

你也可以随时使用git status命令查看文件状态。