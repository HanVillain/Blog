###前言
有段时间没有使用vscode编译markdown文件，今天在写文章时发现提示“Code language not supported or defined.”

![](https://img-blog.csdnimg.cn/2b0ca481c3d0426c9bd3e9bc2aa2c674.png)

百度之后发现可能是需要配置Code run这个插件的一些地方，但是经过试验过后并没有成功，然后自己在想：为什么不直接再一次的重新配置一遍markdown编译环境，因为markdown环境的配置十分简单，所以与其寻找解决办法，不如直接重新配置新的markdown环境

然后百度了一篇最近的vscode配置markdown新环境的文章，发现需要将侧边预览打开
####正文
######侧边预览打开方式
在你的源文件下，鼠标右键呼出预览菜单（或者使用快捷键Ctrl+K V）
![](https://raw.githubusercontent.com/hanread/HanImageBed/main/img/202211091816629.png)
快捷键解释：Ctrl+K然后松开按住V键
注意：右下角语言模式设置为MarkDown否则无法呼出预览（一般情况下code会自动识别出）

这样就可以解决了