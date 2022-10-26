##Git的安装

选择官网进行安装，


##Git的打开

Git的打开方式很简单，我们只需要选择指定的路径，打开这个路径下的文件夹，然后鼠标右键，选择Git Bash Here，就能打开Git，在这里我们并不使用Git Gui Here，因为图形界面并不比代码的输入便捷。当然我们还可以在桌面鼠标右键选择打开Git Bash，通过cd命令跳转到我们想要使用的路径下，不难看出Git Bash和我们windows下的命令行窗口或者Mac下的终端是极其相似的

##Git检测

查看Git是否安装成功

#####方法一
返回桌面右键，选择Git Bash Here，输入
` git -v 或者 git --version `

#####方法二
键盘win + R，输入cmd，在命令行输入
` git -v 或者 git --version `


两种方法只要一个返回git的版本号即视为安装成功。



##Git的配置

#####向Git提交使用者的姓名、邮箱：

######提交姓名
` git config --global user.name "管理员姓名" `

例如
` git config --global user.name "hanread" `

######提交邮箱
` git config --global user.email "管理员邮箱" `

例如
` git config --global user.email "123456789@163.com" `

######检查是否配置成功
` git config --global --list `

出现你配置的仓库管理者的姓名和邮箱即视为配置成功
或者在你C盘的用户目录文件夹下寻找名为.gitconfig的文件，使用记事本打开，是否是你刚刚输入的仓库管理者姓名以及邮箱。

######修改仓库管理者姓名、邮箱只需重复上述操作。


##



