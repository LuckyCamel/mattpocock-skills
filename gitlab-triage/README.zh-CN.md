# gitlab-triage（GitLab Issue 分诊状态机）

## 用途

在当前 GitLab 项目用 **标签状态机** 管理 Issue：创建、分诊、为 AFK 代理准备简报、处理待补充信息等。从 `git remote` 推断项目，用 **`glab`** 操作 GitLab。

## 行为要点

- 须已 `glab auth`；必要时用 `glab issue … -R GROUP/PROJECT` 指定项目。
- 所有发到 Issue 的 **note** 或新建/更新的 **描述** 顶部须带 AI 分诊免责声明（见原 [SKILL.md](./SKILL.md)）。
- Bug 在深入 `/domain-model` 前尽量尝试复现；`ready-for-agent` 需写 agent brief（见 [AGENT-BRIEF.md](./AGENT-BRIEF.md)）。

## 原文

详见 [SKILL.md](./SKILL.md)。
