---
title: VSCode Settings Sync 插件的使用
date: 2019-07-26 11:18:53
tags:
- VSCode
- 插件
---

## 导读

> [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) 是 [VSCode](https://code.visualstudio.com/) 编辑器上的一款插件，可以将当前编辑器所有配置和插件同步到 [GitHub](https://github.com/) 上，以后只需要从 [GitHub](https://github.com/) 上获取，就可以一次性恢复插件和配置。

## 适用于

- Windows 系统
- MacOS 系统
- Ubuntu 系统

## 前序准备

- 下载安装 [VSCode](https://code.visualstudio.com/) 编辑器
- 注册申请 [GitHub](https://github.com/join?source=header-home) 帐号

## 快速开始

### 第一步

- 先在 VSCode 编辑器里面搜索安装 Settings Sync 插件 ，安装好之后重启编辑器加载插件。
![](http://ww4.sinaimg.cn/large/006tNc79ly1g5d34f0n6aj31hc0r2jsx.jpg)

### 第二步

- 按下 Shift + Alt + U （备份）

  - Upload Key : Shift + Alt + U \ Shift ⇧+Option ⌥+ U
  - Download Key : Shift + Alt + D \ Shift ⇧+Option ⌥+ U

- 弹出 Settings Sync 插件界面选择 Login with Github 绑定 GItHub 帐号
![](http://ww2.sinaimg.cn/large/006tNc79gy1g5d855w5e4j31hc0r2acn.jpg)

### 第三步

- 弹出浏览器界面 GitHub 登录界面，输入帐号密码进行下一步确定
![](http://ww3.sinaimg.cn/large/006tNc79gy1g5d87yg51mj31hc0r2q3h.jpg)

### 第四步

- 确定授权之后页面显示成功就可以关闭当前 tab 页面了

  ![](http://ww4.sinaimg.cn/large/006tNc79gy1g5d8a3xqsuj31hc0r2aa8.jpg)

### 第五步

- 回到 VSCode 编辑器会多出一个 tab 窗口点击 Skip 创建新 Gist（以前旧版插件需要到 GitHub 上面手动创建 Gist，现在更新了之后非常方便）

  ![](http://ww1.sinaimg.cn/large/006tNc79gy1g5d8nwl4ufj31hc0r2q4k.jpg)

- 按下 **Shift + Alt + U** 进行当前插件和配置的备份，重装电脑之后或者更换系统之后只需重新下载 VSCode 和 Settings Sync 插件进行以上步骤绑定（如果是已有备份记录的用户只需要选中对应的 Gist ），按下 **Shift + Alt + D** 进行就可以完成 **插件和配置的备份** 恢复了。

  ![](http://ww3.sinaimg.cn/large/006tNc79gy1g5d9x9hejuj31hc0r2jta.jpg)
