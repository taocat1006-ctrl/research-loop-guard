# research-loop-guard

科研止损与迭代守则：让每轮探索产生可判断的知识增量，避免反复补实验、补证据和失败后无限重启。

这是一个以中文编写的 Codex skill，适用于规划下一轮研究、判断继续或停止，以及复盘长期未收敛的研究。普通论文解读和单次代码修复无需套用完整流程。

## 它做什么

- 恢复当前问题、已有结果及最近有效决定，优先复用已有材料。
- 用简短决策卡明确本轮问题、证据、结果对应的行动、预算和停止条件。
- 将预算累计到父问题，区分开发结果、独立验证、技术故障和科学失败。
- 默认在连续两轮只补组件或材料、却未改变父问题决策时停止扩张；用户可事先调整该规则。
- 对已经停止的分支要求具体重启依据；用户明确授权重启后，不重复索要确认。

## 安装

克隆到 Codex 的 skills 目录（若设置了自定义 CODEX_HOME，请使用对应的 skills 目录）：

```bash
git clone https://github.com/taocat1006-ctrl/research-loop-guard.git ~/.codex/skills/research-loop-guard
```

如果目标目录已存在，先保留或备份已有版本，再决定如何合并。重新打开 Codex 会话以加载 skill。

## 使用

在 Codex 中输入：

```text
请使用 $research-loop-guard，结合已有记录判断下一轮科研是否值得做，
并限定本轮问题、预算和停止条件。
```

也可用于“是否陷入补实验循环”“这轮是否该停”“已停止的方向是否有充分理由重启”等请求。

## 文件

- [SKILL.md](SKILL.md)：核心研究决策规则。
- [references/decision-card.md](references/decision-card.md)：单轮决策卡模板。
- [references/behavior-examples.md](references/behavior-examples.md)：通用情境与行为检查。
- [agents/openai.yaml](agents/openai.yaml)：Codex 的显示名称及默认提示。

本仓库是通用发布版本，未包含私人项目记录或本机证据路径。案例仅为示意，不是独立测评。该 skill 限定研究决策，不提供额外执行权限，也不保证研究成功或论文录用。
