# improve-codebase-architecture（架构深化机会）

## 用途

在通读 `CONTEXT.md` 与 `docs/adr/` 的前提下，用统一词汇（Module、Interface、Depth、Seam 等，见 [LANGUAGE.md](./LANGUAGE.md)）指出架构摩擦，提出**深化机会**：把小而浅的模块改成「小接口、厚实现」，提升可测试性与 AI 可读性。

## 流程概要

1. **探索**：先读领域文档与 ADR，再用 Explore 子代理有机扫代码，关注浅模块、耦合泄漏、测试困难处，对可疑模块做「删除测试」。
2. **列出候选**：每条含涉及文件、问题、方案、收益（locality / leverage / 测试改善）；用领域词汇描述，暂不写具体新接口。
3. **拷问循环**：用户选中某条后深入讨论；必要时更新 `CONTEXT.md`、按需提议 ADR；接口形状探索见 [INTERFACE-DESIGN.md](./INTERFACE-DESIGN.md)。

## 原文

详见 [SKILL.md](./SKILL.md)。
