# Clash 从入门到精通

## 前言

Clash 分为两个部分，内核和客户端。
目前经许多大佬贡献，开源社区出现了许多的客户端，
现在已经可以实现一个 Clash 配置跨全部平台使用，
故撰写本文实现最佳实践。

### 内核

原版 Clash 内核已不再维护，现仍在积极维护且广泛使用的内核为 [mihomo](https://github.com/MetaCubeX/mihomo/tree/Alpha) (曾用名 clash meta)。
本文将 旧原版 Clash、clash premium 、mihomo、clash meta 等名字统称为 Clash，实际都是指 [mihomo](https://github.com/MetaCubeX/mihomo/tree/Alpha)。
推荐在使用旧原版 clash、clash premium 内核的用户及时切换到新内核，Clash 兼容旧配置。

### 客户端

客户端功能都是依托于内核，差别不大。

## 第一章 下载安装使用

### 1. 下载客户端

- Windows: [clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev/releases)
- macOS: [clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev/releases)
- Android: [ClashMetaForAndroid](https://github.com/MetaCubeX/ClashMetaForAndroid/releases)
- iOS: 
  > 目前并没有完善好用的开源客户端，仅推荐上架外区 App Store 兼容 Clash 配置的客户端:
  - [Stash](https://stash.ws/) 
  > 美区 $3.99、**不完全兼容 Clash 内核配置**，仅兼容旧的 Premium 内核配置
  - [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)
  > 美区 $2.99，**仅能导入 Clash 配置的节点使用，不能通过配置文件配置**
- Linux: [clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev/releases)
- 其他系统: 推荐直接使用 [mihomo](https://github.com/MetaCubeX/mihomo/tree/Alpha) 内核，面板等不在此处做推荐。

自行下载安装。
### 2. 使用

#### 移动端

使用的方法一般是：

1. 在配置里导入订阅链接
2. 主界面相应按钮点击后启动
3. 按提示允许建立 VPN 连接
4. 状态中心出现 VPN 样式图标说明正在使用中。

桌面端

使用的方法一般是：

1. 双击应用图标打开应用， 一般会在任务栏托盘区显示相应程序的图标
2. 点击托盘区图标显示主界面
3. 在订阅面板里导入订阅链接并选择新导入的订阅
4. 右键单击程序图标勾上**系统代理**
5. 重新打开你需要使用代理的浏览器即可使用

自行探索客户端界面。

**此时已经能满足大部分人日常使用的使用需求了。**

## 第二章 客户端设置

### 1. 移动端

#### Android 设置示例

![android](images/android.png)

其他保持默认，通过配置文件设置即可。

#### iOS 设置示例

- Stash: 参考其官方 [快速上手](https://stash.wiki/get-started) 文档
- Shadowrocket: 参考其官方 [使用教程](https://www.shadowrocket.vip/%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B)

### 2. 桌面端

#### Windows、Linux、macOS 设置示例

![pc](images/pc.png)

其他保持默认。

## 第三章 进阶：配置文件编写

首先，使用 vscode 打开一个空文件夹，里面新建

- config.yaml (Clash 配置文件)
- manual.txt (单个链式服务器节点)
- manual.yaml