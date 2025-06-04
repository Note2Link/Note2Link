# Note2Link桌面客户端端口设置指南

本文档将指导您如何配置Note2Link桌面客户端的端口设置，以便充分利用加速和同步功能。

## 端口设置概述

Note2Link桌面客户端提供两种代理端口设置：
1. **系统代理端口**：用于系统应用程序（如笔记软件）
2. **浏览器代理端口**：用于配合浏览器扩展程序

![Note2Link端口设置界面](./assets/images/port_settings_en-US.png)

## 系统代理端口

系统代理端口用于自动设置系统代理，使笔记软件的加速及同步功能即可用。

- 默认端口：**35777**
- 功能：Note2Link客户端自动设置系统代理，无需手动配置
- 应用场景：各种笔记软件的加速和同步

> **提示**：如果默认端口与其他应用冲突，您可以修改为其他未被占用的端口。

## 浏览器代理端口

浏览器代理端口需要配合浏览器扩展程序使用，以下是配置步骤：

### 推荐使用 Proxy SwitchyOmega 3 (ZeroOmega)

由于各大浏览器逐步停用Manifest V2支持，我们推荐使用**Proxy SwitchyOmega 3 (ZeroOmega)**，简称**ZeroOmega**，它是基于Proxy SwitchyOmega修改而成的插件，支持新版的Manifest V3。

#### ZeroOmega配置步骤：

1. 从浏览器扩展商店安装**Proxy SwitchyOmega 3 (ZeroOmega)**
2. 打开扩展设置界面
3. 创建新的代理配置，设置如下：
   - 代理协议：**SOCKS5**
   - 代理服务器：**127.0.0.1**
   - 代理端口：**35778**（Note2Link默认浏览器代理端口）

![ZeroOmega设置界面](./assets/images/zeroomega_settings_en-US.png)

4. 保存配置并应用

#### 使用方法：

1. 点击浏览器工具栏中的ZeroOmega图标
2. 选择您创建的Note2Link代理配置
3. 现在您的浏览器已通过Note2Link加速

> **注意**：对于从SwitchyOmega迁移过来的用户，ZeroOmega的管理界面几乎一模一样，可以无缝替换。

## 常见问题

### 端口被占用怎么办？

如果默认端口被其他应用占用，您可以在Note2Link设置中修改为其他未被占用的端口，然后相应地更新浏览器扩展的配置。

### 为什么推荐使用ZeroOmega？

因为原版的Proxy SwitchyOmega基于Manifest V2，而各大浏览器正在逐步停止支持此版本。Proxy SwitchyOmega 3 (ZeroOmega)支持Manifest V3，确保您的浏览器扩展能够长期使用。

## 总结

通过正确配置Note2Link的端口设置和浏览器扩展，您可以充分利用Note2Link提供的加速和同步功能，提升笔记软件和浏览器的使用体验。这些设置将帮助您更有效地管理和访问您的笔记内容，无论是在本地应用程序还是在网络浏览过程中。
