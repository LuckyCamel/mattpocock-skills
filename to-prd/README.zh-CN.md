# to-prd（对话上下文 → PRD Issue）

## 用途

基于**当前对话与对仓库的理解**直接产出 **PRD**，并用 **`glab issue create`** 创建 **GitLab Issue**。**不做访谈**，只综合已知信息；实现前会与用户核对模块划分与测试范围意向。

## 流程概要

探索仓库（若尚未）→ 勾勒需新建/修改的模块，寻找可单独测试的 deep modules → 与用户确认模块与测试意向 → 按模板写 Problem、Solution、大量编号 User Stories、Implementation / Testing / Out of scope 等（避免易过期路径与代码片段）→ `glab issue create` 发 issue。

## 原文

详见 [SKILL.md](./SKILL.md)。
