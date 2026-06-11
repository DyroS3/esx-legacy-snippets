# 更新日志

本文件记录「ESX Legacy 代码片段 · 简体中文增强版」的所有重要变更。

## [3.0.0]

简体中文增强版首个版本，在原 ESX 片段基础上进行品牌化、源码对齐与全面中文化。

### 新增
- 基于 [esx-framework/esx_core](https://github.com/esx-framework/esx_core) 的 `es_extended` 源码，补全大量缺失 API：
  - 客户端：`TextUI`/`HideUI`、`Progressbar`、Context 菜单、`Interactions`、`GetShapeTestResultSync`、`RaycastScreen` 等。
  - 回调：`AwaitServerCallback`、`RegisterClientCallback`，以及服务端 `TriggerClientCallback`/`AwaitClientCallback`。
  - 服务端：`OneSync.*`（生成/最近/区域查询全套）、`DiscordLog`、`CreateJob`、`GetItems` 等。
  - 共享：`ESX.Table.*`、`ESX.Math.Random`/`GetHeadingFromCoords`、`ESX.Await`。
  - `xPlayer`：`Meta`（get/set/clear）、`getSource`、`getPlayTime`、`getSSN`、`set`/`get` 等。
- 所有片段加入 Tab 占位符与**简体中文描述**。
- 工程化：新增 `.gitignore`、`.vscodeignore`，以及基于 `@vscode/vsce` 的 GitHub Actions 打包/发布工作流。

### 变更
- 品牌信息改为社区增强版：`displayName`、`description`、`publisher`、`repository` 等均更新。
- 全部用户可见文本中文化（显示名、简介、片段描述、README、CHANGELOG）。
- 片段数量由 138 增至 205。

### 修复
- 修正过时签名与错误命名，例如：
  - `ESX.Game.GetVehicleDirection` → `ESX.Game.GetVehicleInDirection()`
  - `ESX.Game.GetPedMugShot` → `ESX.Game.GetPedMugshot(ped, transparent)`
  - `ESX.Scaleform.RequestScaleformMovie` → `ESX.Scaleform.Utils.RequestScaleformMovie`
  - `xPlayer.getCoords` / `setJob` / `addMoney` / `showNotification` 等签名更新。
- 修正若干片段的语法错误（缺失括号、`Steaming` 拼写、`RegisterType` 命名空间等）。

---

## 历史版本（原 ESX 片段）

### [2.0.1]
- 修正扩展信息。

### [1.0.2]
- 更新部分片段。

### [1.0.1]
- 更新 README.md。

### [1.0.0]
- 初始发布。
