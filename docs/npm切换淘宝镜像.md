由于官方npm的包服务器在国外，对于国内用户，在不借助梯子的情况下可能会下载缓慢，甚至下载失败，这个时候我们就可以将替换为国内的镜像源，例如淘宝提供的镜像源`https://registry.npm.taobao.org`。

淘宝为我们搭建了一个国内的npm服务器，它目前是每隔10分钟将国外npm仓库的所有内容“搬运”回国内的服务器上，这样我们直接访问淘宝的国内服务器就可以了，它的地址是：https://registry.npm.taobao.org


方法一：npm install -g cnpm --registry=https://registry.npm.taobao.org

检查是否安装成功：
`cnpm -v`
cnpm是国内对npm的镜像版本，使用阿里定制的cnpm命令行工具代替默认的npm,安装成功之后，以后安装依赖包的方式和npm的是一样的，只是npm的命令换成是cnpm就可以了。
例如原生npm命令为：npm install uniq --save，cnpm命令为：cnpm install uniq --save



方法二：
单次使用：
`npm install --registry=https://registry.npm.taobao.org`

永久替换：

在开发react-native的时候，不要使用cnpm，cnpm安装的模块路径比较奇怪，packager不能正常识别。

所以，为了方便开发，我们最好是直接永久使用淘宝的镜像源

直接命令行的设置
npm config set registry https://registry.npm.taobao.org
手动修改设置

1.打开.npmrc文件（C:\ProgramFiles\nodejs\node_modules\npm\npmrc，没有的话可以使用git命令行建一个( touch .npmrc)，用cmd命令建会报错）
2.增加 registry =https://registry.npm.taobao.org  即可。
如果需要恢复成原来的官方地址只需要执行如下命令:

npm config set registry https://registry.npmjs.org
检测是否安装成功：

npm config get registry

以后安装时，依然用npm命令，但是实际是从淘宝国内服务器下载的