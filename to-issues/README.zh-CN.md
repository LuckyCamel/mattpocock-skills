# to-issues（计划拆成 GitLab Issue）

## 用途

把已有计划、规格或 PRD 拆成可独立领取的 **GitLab Issue**，每条是 **tracer bullet 式竖切**（贯穿各层、可单独演示/验收），并区分 **HITL**（需人参与）与 **AFK**（可无人值守做完）。

## 流程概要

收集上下文（可从对话或 `glab issue view <iid> --comments`）→ 可选探索代码 → 起草切片列表（标题、类型、阻塞、覆盖的用户故事）→ **测验用户** 粒度与依赖是否合适 → 按依赖顺序 `glab issue create`，使用 skill 内 issue 模板；不要关闭或改动父 issue。

## 原文

详见 [SKILL.md](./SKILL.md)。
