# J1ntttao 的 Dalamud 插件源

个人维护的《最终幻想 XIV》Dalamud 第三方插件源。

## 插件源地址

在 Dalamud 的自定义插件仓库中添加：

```text
https://raw.githubusercontent.com/J1ntttao/FFXIVDalamudPlugins/master/pluginmaster.json
```
## 添加方法

1. 在游戏中输入 `/xlsettings` 打开 Dalamud 设置。
2. 进入“实验性功能”或 `Experimental` 页面。
3. 找到“自定义插件仓库”或 `Custom Plugin Repositories`。
4. 添加上面的 `pluginmaster.json` 地址。
5. 保存设置并刷新插件列表。
6. 在插件安装器中搜索需要的插件。

如果插件源无法加载，请先在浏览器中打开插件源地址，确认能够正常显示 JSON 内容。

## 仓库现有插件

### Triad Buddy Auto

- 当前版本：`1.0.0.8`
- 作者：`J1ntttao`
- Dalamud API：`15`
- Triad Buddy：`1.15.0.1`
- Bug 反馈：`qq2379873505@163.com`

主要功能：

- 读取 Triad Buddy 的 NPC 幻卡求解结果。
- 自动执行求解器推荐的落牌动作。
- 连续再战时自动点击“再战”和“挑战”。
- 在连续再战的选卡阶段自动选择最优卡组。
- 支持观察模式、动作稳定检查和 `Pause` 紧急停止。
- 玩家手动拖牌时暂停自动操作；有效落牌让出当前步，无效拖放在 500 毫秒冷却后重新等待推荐。
- Triad Buddy 检测到 PVP 对战时同步状态且不接管对局。
- 幻卡棋盘显示期间自动保持完整插件窗口打开。

插件不会主动寻找 NPC 或发起第一次挑战，仅接管 NPC 幻卡对局。

### Better Fake Name

- 当前版本：`1.3.0.0`
- 作者：`J1ntttao`
- Dalamud API：`15`
- 源码：[J1ntttao/FFXIV_BetterFakeName](https://github.com/J1ntttao/FFXIV_BetterFakeName)
- Bug 反馈：`qq2379873505@163.com`

主要功能：

- 自定义原生 UI 中的玩家姓名、称号、部队简称和区服。
- 支持从当前目标或手动输入快速添加映射。
- 支持配置导入导出，方便备份和迁移。

插件只改变本机显示，不修改服务端资料、游戏对象、网络数据或玩家链接中的真实身份。

## 免责声明

本仓库中的插件均为第三方工具，与 Square Enix 和 Dalamud 官方无关。第三方插件及自动操作可能违反游戏服务条款，请自行评估并承担使用风险。

插件完全免费，请勿在任何地方付费购买。
