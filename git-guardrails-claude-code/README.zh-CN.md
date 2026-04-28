# git-guardrails-claude-code（Claude Code Git 护栏）

## 用途

为 Claude Code 配置 **PreToolUse** 钩子，在执行前拦截危险 `git` 命令（如 `git push`、`reset --hard`、`clean`、`branch -D`、`checkout .` / `restore .` 等），降低误操作风险。

## 工作流概要

1. 询问范围：**仅当前项目**（`.claude/settings.json`）还是**全局**（`~/.claude/settings.json`）。
2. 将 [scripts/block-dangerous-git.sh](./scripts/block-dangerous-git.sh) 复制到对应 hooks 目录并赋予执行权限。
3. 把钩子合并进 settings（勿覆盖其他 hooks）。
4. 可按用户要求增删拦截模式。
5. 用 skill 内文档中的 `echo '...' | script` 方式自测应返回退出码 2 与 BLOCKED 信息。

## 说明

脚本与示例路径偏 Unix；在 Windows 上需结合 WSL 或 Claude Code 实际运行环境调整。

## 原文

详见 [SKILL.md](./SKILL.md)。
