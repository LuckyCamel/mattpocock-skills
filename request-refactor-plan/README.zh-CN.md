# request-refactor-plan（重构计划访谈 + GitLab Issue）

## 用途

通过多轮访谈与仓库核对，把重构动机、备选方案、范围、测试策略敲实，再拆成**极小步可提交**的提交计划，最终以固定模板用 **`glab issue create`** 发成 **GitLab Issue**（类似重构 RFC）。

## 步骤概要

收集问题描述 → 探索验证 → 讨论备选 → 细访实现细节 → 划定改/不改边界 → 看测试覆盖并问测试打算 → 按 Fowler「每步尽量小且可运行」列 commits → 用模板写 Problem / Solution / Commits / Decision / Testing / Out of scope 等（避免易过期的文件路径与代码片段）。

## 原文

详见 [SKILL.md](./SKILL.md)。
