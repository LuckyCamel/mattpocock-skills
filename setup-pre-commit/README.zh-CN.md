# setup-pre-commit（Husky 预提交）

## 用途

在当前仓库配置 **Husky** 预提交：**lint-staged**（Prettier 写回暂存文件）、以及（若存在脚本）**typecheck** 与 **test**。

## 步骤概要

检测包管理器 → 安装 `husky`、`lint-staged`、`prettier` → `npx husky init` → 写 `.husky/pre-commit`（按包管理器替换命令，无 typecheck/test 则省略）→ `.lintstagedrc` → 若无 Prettier 配置则创建默认 `.prettierrc` → 验证 → 用约定消息提交。

## 原文

详见 [SKILL.md](./SKILL.md)。
