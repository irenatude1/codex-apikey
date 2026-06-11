
# Codex 配置 API Key 教程：中转站注册、密钥创建与覆盖配置完整指南

本教程主要介绍如何为 Codex 配置 API Key，适合国内用户使用 Codex CLI、Codex App、VS Code Codex 插件等工具时参考。

通过本文，你可以完成：

- 注册 Codex 中转站
- 创建 Codex API Key
- 选择正确的模型分组
- 使用覆盖配置脚本完成 Codex 配置
- 启动 Codex CLI 并开始使用

---

## 01. Codex 中转站地址

本文使用的 dkai-codex 中转站地址如下：

[dkai-codex 中转站注册地址](https://codex.dakeai.cc/register?promo=DKAI)

该站点主要面向 Codex、Claude Code 等编程工具调用场景。

如果你还有 OpenClaw 或其他支持第三方自定义 API 接入的 Agent、AI 程序调用需求，也可以使用 dkapi：

[dkapi 通用 API 中转站](https://api.dakeai.cc)

dkapi 支持多种常见兼容协议，一个 Key 可以调用多款大模型。使用时通常只需要根据兼容协议替换 URL 和 Key 即可。

---

## 02. 使用前需要准备什么？

中转站使用主要分为两个关键步骤：

1. 安装对应工具平台  
2. 覆盖 Codex 配置

如果你已经安装过 Codex App、Codex CLI 或 VS Code Codex 插件，可以跳过安装步骤，直接进行后面的覆盖配置。

如果你还没有安装，可以先参考：

- [Codex Desktop App 下载安装与配置教程](https://dk82.com/635.html)
- [VS Code Codex 插件安装教程](https://zhuanlan.zhihu.com/p/2035752399952950892)
- [Codex App 配置画图 API 教程](https://dk82.com/714.html)

---

## 03. 注册并创建 API 密钥

注册并登录中转站后，进入 API 密钥页面。

操作步骤如下：

1. 打开 API 密钥页面
2. 点击创建密钥
3. 填写密钥名称
4. 选择对应分组
5. 保存并生成 API Key

![创建 API 密钥界面](https://dk82.com/wp-content/uploads/2026/03/d2b5ca33bd200429-1024x450.png)

---

## 04. 分组应该怎么选择？

创建密钥时，密钥名称可以自定义填写，但分组必须选择正确。

不同分组对应不同模型和工具：

- **Codex 分组**：适合 Codex CLI、Codex App、VS Code Codex 插件等工具
- **Claude 分组**：适合 Claude Code 相关工具

如果你要配置的是 Codex，建议选择 **Codex 分组**。

![分组选择说明](https://dk82.com/wp-content/uploads/2026/03/d2b5ca33bd200609-1024x915.png)

---

## 05. 使用密钥并获取覆盖配置脚本

以 Codex 为例，创建好 Codex 分组密钥后，在密钥列表中找到刚刚创建的密钥。

点击密钥右侧的 **使用密钥**，进入配置说明页面。

![使用密钥入口](https://dk82.com/wp-content/uploads/2026/03/d2b5ca33bd200959-1024x213.png)

进入后，根据你的操作系统选择对应方法：

- Windows 用户可以选择 PowerShell 或 CMD 相关配置方式
- macOS / Linux 用户可以选择终端配置方式

如果你还没有安装对应工具，可以先执行安装步骤。

如果已经安装完成，可以直接执行 **覆盖配置**。

---

## 06. 执行覆盖配置脚本

覆盖配置是整个教程中最关键的一步。

操作方法：

1. 在“使用密钥”页面找到覆盖配置脚本
2. 点击复制脚本
3. 打开终端
4. 粘贴脚本并执行
5. 等待提示配置成功
6. 重启 Codex CLI、Codex App 或 VS Code 插件

![配置脚本界面](https://dk82.com/wp-content/uploads/2026/03/d2b5ca33bd201150-1024x691.png)

![终端执行示例](https://dk82.com/wp-content/uploads/2026/03/d2b5ca33bd201411-1024x465.png)

配置成功后，Codex 会使用新的 API Key 和中转接口地址进行调用。

---

## 07. 启动 Codex CLI 测试

安装并覆盖配置完成后，就可以启动 Codex CLI 进行测试。

不同系统打开终端方式如下：

- macOS 用户：打开 Terminal
- Linux 用户：打开终端
- Windows 用户：打开 CMD 或 PowerShell

然后输入：

```bash
codex
````

按回车后即可启动 Codex CLI。

第一次进入时，可能会出现几个提示，一般直接按回车即可。

启动成功后，你可以直接在界面中输入问题，例如：

```text
帮我写一个简单的个人博客首页
```

或者：

```text
帮我检查这个 Python 脚本为什么报错
```

---

## 08. 配置完成后可以做什么？

配置完成后，你可以使用 Codex 完成很多编程相关任务，例如：

* 生成网页代码
* 修改已有项目
* 解释代码逻辑
* 排查报错原因
* 重构代码结构
* 编写脚本和自动化工具
* 辅助完成网站、小程序、桌面应用等项目

如果你不知道怎么使用，也可以直接问 Codex：

```text
我完全不会写代码，想做一个简单的网站，你能一步步教我吗？
```

安装好以后，不怕不会用，关键是多提需求、多尝试。

---

## 09. 总结流程

完整流程如下：

```text
注册中转站 → 创建 API 密钥 → 选择 Codex 分组 → 点击使用密钥 → 复制覆盖配置脚本 → 终端执行 → 重启工具 → 开始使用
```

完成以上步骤后，Codex CLI、Codex App 或 VS Code Codex 插件就可以正常调用中转 API 使用了。

```
```
