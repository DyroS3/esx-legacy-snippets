<h1 align="center">ESX Legacy 代码片段 · 简体中文增强版</h1>

<p align="center">
  为 <a href="https://github.com/esx-framework/esx_core">ESX Legacy（es_extended）</a> 框架打造的 Visual Studio Code 代码片段扩展。<br/>
  所有界面文本均为<b>简体中文</b>，片段签名与最新 <code>esx_core</code> 源码保持一致。
</p>

---

## 简介

这是 ESX Legacy 代码片段扩展的**简体中文增强版**。在你编写 FiveM / ESX 资源时，输入 `ESX.` 或 `xPlayer.` 等前缀即可自动补全对应的函数调用，并带有 **Tab 占位符**与**中文说明**，帮助你更快、更准地写代码。

> 本扩展是社区维护的增强版本，并非 ESX 官方发布。片段内容依据 [esx-framework/esx_core](https://github.com/esx-framework/esx_core) 的 `es_extended` 源码整理与核对。

## 特性

- ✅ **与源码对齐**：依据最新 `esx_core` 源码核对每个函数签名，修正了大量过时/错误的签名与命名。
- ✅ **全中文说明**：每个片段都带有简体中文描述，悬停/补全时一目了然。
- ✅ **Tab 占位符**：参数以 `${1:param}` 形式提供，按 <kbd>Tab</kbd> 快速跳转填写。
- ✅ **覆盖全面**：客户端 / 服务端 / 共享，共 **200+** 个片段，涵盖 `ESX.*`、`ESX.Game.*`、`ESX.OneSync.*`、`ESX.UI.Menu.*`、`ESX.Streaming.*`、`ESX.Scaleform.*`、`ESX.Table.*`、`ESX.Math.*`、回调、`xPlayer.*` 等。

## 安装

**方式一：从 VS Code 扩展市场安装**

在扩展面板中搜索「ESX Legacy 代码片段」或「ESX 简体中文」，点击安装。

**方式二：本地安装 VSIX**

```bash
# 在项目根目录打包
npm install
npm run package
# 然后在 VS Code 中：扩展面板 → 右上角 ... → 从 VSIX 安装
```

## 使用方法

1. 打开任意 `.lua` 文件。
2. 输入片段前缀，例如：
   - `ESX.RegisterServerCallback`
   - `xPlayer.addMoney`
   - `ESX.Game.SpawnVehicle`
3. 从补全列表中选择，按 <kbd>Tab</kbd> 在参数占位符之间跳转填写。

> 提示：前缀即真实函数名，因此即使忘记完整写法，输入 `ESX.Game.` 也能列出该命名空间下的所有片段。

## 片段速查（按命名空间）

| 命名空间 | 范围 | 示例前缀 |
| --- | --- | --- |
| `ESX.*`（客户端） | 通知 / UI / 玩家数据 | `ESX.ShowNotification`、`ESX.TextUI`、`ESX.GetPlayerData` |
| `ESX.Game.*` | 实体 / 载具 / 生成 | `ESX.Game.SpawnVehicle`、`ESX.Game.GetClosestPlayer` |
| `ESX.UI.Menu.*` | 旧版菜单 | `ESX.UI.Menu.Open`、`ESX.UI.Menu.RegisterType` |
| `ESX.Streaming.*` | 资源加载 | `ESX.Streaming.RequestModel` |
| `ESX.Scaleform.*` | Scaleform | `ESX.Scaleform.ShowFreemodeMessage` |
| 回调 | 客户端 / 服务端回调 | `ESX.RegisterServerCallback`、`ESX.TriggerServerCallback` |
| `ESX.*`（服务端） | 玩家 / 物品 / 工作 | `ESX.GetPlayerFromId`、`ESX.RegisterUsableItem` |
| `ESX.OneSync.*` | 服务端生成 / 查询 | `ESX.OneSync.SpawnVehicle` |
| `ESX.Math.*` / `ESX.Table.*` | 工具函数 | `ESX.Math.Round`、`ESX.Table.Filter` |
| `xPlayer.*` | 玩家对象方法 | `xPlayer.addMoney`、`xPlayer.setJob` |

## 贡献

欢迎提交 Issue 与 Pull Request：

- 仓库：<https://github.com/DyroS3/esx-legacy-snippets>
- 问题反馈：<https://github.com/DyroS3/esx-legacy-snippets/issues>

## 许可证

基于 [MIT License](LICENSE.md) 开源。原始片段版权归 ESX 社区所有，本增强版在其基础上整理、修正并中文化。
