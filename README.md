## 介绍

一个使用`aardio`开发的用于绕过冒险岛079版本的MAC机器码黑名单的工具。

不保证所有079的客户端都能正常绕过。

能用便用吧，不更新维护。

## 功能

- 绕过服务端所限制的MAC机器码多开
- 绕过服务端所限制的MAC机器码黑名单

## 原理

在`MapleStory.exe`客户端文件中找到登录时填充账号密码以及发送`MAC`机器码的`CALL`,对填充`MAC`机器码部分进行`InlineHook`，随机生成`MAC`机器码后正常发包。
__仅HOOK登录界面的Call。__

## 使用方法

打开后，按住程序中间的手套状图标拖动到目标窗口即可。

![主程序图片展示](./img_show/show.png)

__注意:为了使多开生效,请在登录之前完成此操作，否则使用的是你本机生成的MAC。__

## 手动编译本项目

1. 前往[aardio官网](https://www.aardio.com/)下载IDE
2. `git clone https://github.com/Gccc9/MapleStory079_MAC_Bypass.git`
3. 使用IDE打开`default.aproj`并点击编译
4. 找到`dist`目录下的`exe`文件打开即可。


