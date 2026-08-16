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

- 当前版本：`1.0.0.3`
- 作者：`J1ntttao`
- Dalamud API：`15`
- Triad Buddy：`1.15.0.1`
- 源码：[J1ntttao/FFXIV_TriadBuddyAuto](https://github.com/J1ntttao/FFXIV_TriadBuddyAuto)
- Bug 反馈：`qq2379873505@163.com`

主要功能：

- 读取 Triad Buddy 的 NPC 幻卡求解结果。
- 自动执行求解器推荐的落牌动作。
- 连续再战时自动点击“再战”和“挑战”。
- 在连续再战的选卡阶段自动选择最优卡组。
- 支持观察模式、动作稳定检查和 `Pause` 紧急停止。
- 支持显示累计下载请求数和用户自愿参与的匿名在线人数。

插件不会主动寻找 NPC 或发起第一次挑战，仅支持 NPC 幻卡对局。

## 仓库结构

```text
FFXIVDalamudPlugins/
├─ pluginmaster.json
├─ README.md
├─ statistics-server/
│  └─ README.md
└─ plugins/
   └─ TriadBuddyAuto/
      └─ latest.zip
```

- `pluginmaster.json`：Dalamud 读取的插件索引。
- `plugins/<插件名>/latest.zip`：插件安装包。
- `statistics-server/`：部署在 ARM64 Ubuntu 开发板上的下载量与匿名在线人数统计服务；部署及接入方式见目录内 README。

## 直接链接

插件索引：

```text
https://raw.githubusercontent.com/J1ntttao/FFXIVDalamudPlugins/master/pluginmaster.json
```

Triad Buddy Auto 安装包：

```text
https://stats.j1ntao.icu/download?channel=install
```

## 免责声明

本仓库中的插件均为第三方工具，与 Square Enix 和 Dalamud 官方无关。第三方插件及自动操作可能违反游戏服务条款，请自行评估并承担使用风险。

插件完全免费，请勿在任何地方付费购买。
