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

## 当前插件

### Triad Buddy Auto

- 当前版本：`0.2.0.0`
- 作者：`J1ntttao`
- Dalamud API：`15`
- Triad Buddy：`1.15.0.1`
- 源码：[J1ntttao/FFXIV_TriadBuddyAuto](https://github.com/J1ntttao/FFXIV_TriadBuddyAuto)
- Bug 反馈：`2379873505@163.com`

主要功能：

- 读取 Triad Buddy 的 NPC 幻卡求解结果。
- 自动执行求解器推荐的落牌动作。
- 连续再战时自动点击“再战”和“挑战”。
- 在连续再战的选卡阶段自动选择最优卡组。
- 支持观察模式、动作稳定检查和 `Pause` 紧急停止。

插件不会主动寻找 NPC 或发起第一次挑战，仅支持 NPC 幻卡对局。

## 仓库结构

```text
FFXIVDalamudPlugins/
├─ pluginmaster.json
├─ README.md
└─ plugins/
   └─ TriadBuddyAuto/
      └─ latest.zip
```

- `pluginmaster.json`：Dalamud 读取的插件索引。
- `plugins/<插件名>/latest.zip`：插件安装包。

## 直接链接

插件索引：

```text
https://raw.githubusercontent.com/J1ntttao/FFXIVDalamudPlugins/master/pluginmaster.json
```

Triad Buddy Auto 安装包：

```text
https://raw.githubusercontent.com/J1ntttao/FFXIVDalamudPlugins/master/plugins/TriadBuddyAuto/latest.zip
```

## 发布更新

更新插件时需要同时完成以下操作：

1. 在插件源码项目中提升程序集版本。
2. 执行 Release 编译和测试。
3. 使用新产物替换 `plugins/TriadBuddyAuto/latest.zip`。
4. 将 `pluginmaster.json` 中的 `AssemblyVersion` 更新为相同版本。
5. 提交并推送插件索引和安装包。

示例：

```powershell
git add README.md pluginmaster.json plugins/TriadBuddyAuto/latest.zip
git commit -m "release: Triad Buddy Auto 0.2.0.0"
git push origin master
```

## 免责声明

本仓库中的插件均为第三方工具，与 Square Enix 和 Dalamud 官方无关。第三方插件及自动操作可能违反游戏服务条款，请自行评估并承担使用风险。

插件完全免费，请勿在任何地方付费购买。
