# write-a-skill（编写 Agent Skill）

## 用途

指导如何新建 **Claude/Cursor 等可用的 Skill**：收集需求 → 起草 `SKILL.md`（及可选 REFERENCE、脚本）→ 与用户评审。强调 **YAML  frontmatter 里的 `description`** 是代理**唯一**用于判断是否加载该 skill 的线索，必须写清能力与触发词（「Use when…」）。

## 结构约定

- 主说明放 `SKILL.md`；过长或不同领域可拆文件；确定性操作用脚本。
- 建议 `SKILL.md` 控制在约 100 行内（复杂内容外链）；描述 ≤1024 字符、第三人称。

## 原文

详见 [SKILL.md](./SKILL.md)。
