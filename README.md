# Clash 从入门到精通

## 前言

Clash 分为两个部分，内核 和 客户端。

### 内核

原版 Clash 内核已不再维护，现仍在积极维护且广泛使用的内核为 [mihomo](https://github.com/MetaCubeX/mihomo/tree/Alpha) (曾用名 clash meta)。
本文将 Clash 、mihomo、clash meta 等名字统称为 Clash，实际都是指 [mihomo](https://github.com/MetaCubeX/mihomo/tree/Alpha)。
推荐在使用旧版 clash、clash premium 内核的用户及时切换到新内核，Clash 兼容旧配置。

### 客户端

为便于图形化操作使用内核于是衍生出许多第三方客户端。功能都是依托于内核，差别不大。

## 入门

### 第一章 下载安装使用

#### 1. 推荐客户端

##### 下载链接：

Windows: [clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev/releases)
MacOS: [clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev/releases)
Android: [ClashMetaForAndroid](https://github.com/MetaCubeX/ClashMetaForAndroid/releases)
iOS: 
- [Stash](https://stash.ws/) (美区 $3.99、**不完全兼容 Clash 内核**，[使用文档](https://stash.wiki/))
- [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)(美区 $2.99，**仅能导入 Clash 配置的节点使用，不能通过配置文件配置**)
Linux: [clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev/releases)
其他: [mihomo](https://github.com/MetaCubeX/mihomo/tree/Alpha)

自行下载安装。
#### 2. 使用

##### 移动端

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

### 第二章 进阶：客户端设置

#### 移动端

##### Android 设置示例

![android](images/android.png)

其他保持默认，通过配置文件设置即可。

##### iOS 设置示例

待补充