---
title: 导入节点到 Qv2ray
---

# 第三步：导入节点到 Qv2ray

Qv2ray 支持多种方式导入您的配置。为了让您入门，我们挑选了这些最常见的用例：

## 分享链接

> 共享链接一般看起来像这样：
> 
> - `vmess://`...
> - `ss://`...

按照这些步骤导入它们：

1. 点击 **主窗口中的导入** 按钮，或通过 [链接导入](qv2ray://open/import/link)。
2. 在 **导入文件** 对话框中，选择导入源 **共享链接**
3. 将您的分享链接粘贴到 **分享链接** 文本框。
4. 点击 **导入** 按钮来完成。

:::tip 批量导入

您可以一次导入多个分享链接。请确保每行只有一条链接。

:::

:::warning 坏掉的链接

某些已坏掉的分享链接可能无法导入，但它并不重要。详细的错误将显示在右侧。此外，它不会停止批量导入其他条目。

:::

## 订阅

> 订阅链接通常看起来像这样： `https://some-airport.domain/links/YjYyODk?sub=3`

要导入一个订阅，请遵循以下步骤：

1. 在主窗口中点击 **组编辑器** 按钮打开 **组编辑器**
2. 点击 **在左下角添加** 组图标按钮 **[组编辑器](qv2ray://open/group/connection)** 窗口。
3. 选择 **分组列表**中创建的项目，其详细信息将显示在右侧。
4. 切换到 **订阅设置** 面板并完成配置：
   1. 编辑 **分组名称**。
   2. 勾选 **此组是一个订阅**。
   3. 设置以下字段：
      - **订阅地址**：使用上面提到的 **订阅链接**
      - **订阅类型**：如果默认值无法工作，请将其更改为另一值。
   4. 可选更改这些字段：
      - **更新间隔**：当订阅需要在启动时更新时，Qv2ray 会通知您。根据您自己的要求更改它。
      - **导入过滤器**：Qv2ray 可以过滤从您的订阅中导入的节点。你可以自己研究出使用方法。
5. 点击 **更新订阅** 按钮并等待完成。
6. 点击 **确定** 应用设置并关闭对话框。

:::tip 通过系统代理更新

如果您在上游订阅时遇到连接问题，(例如 DNS 记录污染、IP 地址拦截等)，您可以尝试使用 **更新系统代理** 选项的订阅。然而，更好的方法是尽快通知上游，以便永久解决这一问题。

:::

## 手动配置

1. 在主窗口左下角点击 **新建**。
2. 填写 **名称/前缀** 或留空，或者您可以在完成配置后重命名它。
3. 点击 **手动输入** -> **打开连接编辑器**。
4. 填写 **Tag**。此标签将出现在日志中。你也可以留空。
5. 填写 **主机** 并选择您的代理类型。
6. 配置 **杂项设置** 可选。
7. 填写 **出站设置** 和 **流设置**。
8. 点击 **确定** 保存您的配置。

## 导入现有配置

如果您使用 v2ray-core，您可以导入现有的配置文件。**高级** -> **选择**，或 **打开 JSON 编辑器** 并粘贴它。

:::warning 关于首选项设定失效

如果你使用复杂配置，Qv2ray 会忽略首选项中的设定（例如路由设定等）。

:::
