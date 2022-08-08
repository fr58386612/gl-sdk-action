# siflower-sdk-action
使用教程请参考以下链接
https://forum.gl-inet.cn/forum.php?mod=viewthread&tid=539&extra=page%3D1


为了帮助大家编译插件，我做了一个基于github action的插件库,可以帮助大家自动编译出需要的插件
当前支持型号:
AXT1800
SF1200
SFT1200

前置条件:
1. 自己必须注册github账号
2. github账号需使能action，action使能请参考github官方文档

Action仓库链接：
https://github.com/luochongjun/gl-sdk-action

## 使用教程:
1. fork我的x项目到自己仓库



2. fork之后会自动切到自己的仓库
   . 切到Action页面
   . 选择set_variable 工作流
   . 点击run workflow按钮   . 选择需要编译的目标设备
   . 在下拉输入框source code URL中填入需要编译的插件源码地址（注意使用https，不要使用ssh, 例：https://github.com/luochongjun/edgerouter.git ）
   . 在下拉输入框Openwrt package name中填入需要编译的插件名 （要编译的插件名字，例：edgerouter）
   .  如果源代码需要认证信息可以输入邮箱和密码，如果没有则留空
   . 点击Run workflow


3. 接下来会自动执行编译，编译时间快的可能2，3分钟，取决于插件本身的编译时间


4. 编译完成后，点击对应工作，可查看编译好的插件压缩包，压缩包中包含了你需要编译的插件以及所有依赖软件包

下载解压后找到需要的ipk文件


5. 将ipk文件传到路由器后台，使用opkg命令安装.




本主题由 萝卜大侠 于 6 天前 置顶
下载.png (129.72 KB, 下载次数: 0)

下载.png
