# triage-issue（Bug 分诊 + TDD 修复计划 Issue）

## 用途

用户描述问题后**尽量少问**（必要时只问一句「看到什么现象？」），用 Explore 深挖代码找**根因**，再用 **`glab issue create`** 创建 GitLab Issue：含现象/期望/复现、**根因分析**（用模块与行为描述，避免绑定当前路径行号）、以及 **按 RED-GREEN 竖切** 的 TDD 修复步骤与验收标准。

## 原则

- Issue 应在大重构后仍可读：写行为与契约，不写易碎实现细节。
- 测试计划遵守本仓库 TDD skill 的竖切与公开接口取向。

## 原文

详见 [SKILL.md](./SKILL.md)。
