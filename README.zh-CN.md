# Agent Skills 仓库说明（中文）

本仓库收录多份面向 **Claude Code / Agent** 的 **Skill**（以各目录下的 `SKILL.md` 为准）。英文总览与安装命令见根目录 [README.md](./README.md)。

每个子目录是一个独立 skill；**中文说明**放在同目录的 **`README.zh-CN.md`**，便于快速了解用途与工作流，细节仍以 `SKILL.md` 原文为准。

## 关于本 fork

本仓库 **fork 自** [https://github.com/mattpocock/skills](https://github.com/mattpocock/skills)。

相对上游，本 fork 做了如下约定：**工单平台由 GitHub 改为 GitLab**，相关 skill 中的命令由 **`gh`（GitHub CLI）** 改为 **`glab`（GitLab CLI）**（例如 Issue 的创建、查看、列表、评论、标签更新与关闭等）；原 **`github-triage`** skill 目录重命名为 **`gitlab-triage`**。使用本 fork 前请安装并配置好 `glab`（如 `glab auth login`），并确保工作副本的 `git remote` 指向正确的 GitLab 项目。若需与上游 Matt 的原始行为完全一致，请以官方仓库的 `SKILL.md` 为准或直接使用上游安装路径。

---

## 规划与设计

| Skill | 中文说明 |
| ----- | -------- |
| [to-prd](./to-prd/README.zh-CN.md) | 把当前对话与代码理解整理成 PRD，并用 `glab` 创建 GitLab Issue（不额外访谈）。 |
| [to-issues](./to-issues/README.zh-CN.md) | 把计划/PRD 拆成竖切、可独立领取的 GitLab Issue（HITL/AFK），用 `glab issue create`。 |
| [grill-me](./grill-me/README.zh-CN.md) | 对计划/设计高强度追问，逐决策树澄清，每题带推荐答案。 |
| [domain-model](./domain-model/README.zh-CN.md) | 结合领域模型拷问方案，并维护 `CONTEXT.md` / 按需 ADR。 |
| [design-an-interface](./design-an-interface/README.zh-CN.md) | 并行多方案设计模块接口，对比后再综合（Design it twice）。 |
| [request-refactor-plan](./request-refactor-plan/README.zh-CN.md) | 访谈式重构规划 + 极小步提交列表，用 `glab` 落成 GitLab Issue。 |
| [zoom-out](./zoom-out/README.zh-CN.md) | 要求从更高抽象层给出模块与调用关系地图。 |

---

## 开发与工程实践

| Skill | 中文说明 |
| ----- | -------- |
| [tdd](./tdd/README.zh-CN.md) | 红绿重构、竖切 tracer bullet，测试对齐公开行为。 |
| [triage-issue](./triage-issue/README.zh-CN.md) | 调查 bug 根因，用 `glab` 开带 TDD 修复计划的 durable GitLab issue。 |
| [improve-codebase-architecture](./improve-codebase-architecture/README.zh-CN.md) | 结合 `CONTEXT.md` / ADR 找架构「深化」机会与可测性改进。 |
| [migrate-to-shoehorn](./migrate-to-shoehorn/README.zh-CN.md) | 测试里用 shoehorn 替代不安全 `as` 断言。 |
| [scaffold-exercises](./scaffold-exercises/README.zh-CN.md) | 按 lint 规则生成课程练习目录结构。 |
| [qa](./qa/README.zh-CN.md) | 交互式 QA，后台扫代码，用 `glab` 直接创建用户向、行为向的 GitLab Issue。 |

---

## 工具与协作

| Skill | 中文说明 |
| ----- | -------- |
| [setup-pre-commit](./setup-pre-commit/README.zh-CN.md) | Husky + lint-staged + Prettier，可选 typecheck/test。 |
| [git-guardrails-claude-code](./git-guardrails-claude-code/README.zh-CN.md) | Claude Code 钩子拦截危险 git 命令。 |
| [gitlab-triage](./gitlab-triage/README.zh-CN.md) | 用标签状态机分诊与管理 GitLab Issue（`glab`）。 |

---

## 写作与知识

| Skill | 中文说明 |
| ----- | -------- |
| [write-a-skill](./write-a-skill/README.zh-CN.md) | 新 skill 的结构、`description` 写法与拆分原则。 |
| [edit-article](./edit-article/README.zh-CN.md) | 按信息依赖重组文章，分段重写并控制段落长度。 |
| [ubiquitous-language](./ubiquitous-language/README.zh-CN.md) | 从对话抽取术语表，写入 `UBIQUITOUS_LANGUAGE.md`。 |
| [obsidian-vault](./obsidian-vault/README.zh-CN.md) | Obsidian 库内搜索/创建/链接笔记（路径需按环境改写）。 |

---

## 沟通与风格

| Skill | 中文说明 |
| ----- | -------- |
| [caveman](./caveman/README.zh-CN.md) | 极简压缩回复模式，显著减少客套与冗余 token。 |

---

## 安装（与英文 README 一致）

各 skill 可通过官方 skills 工具添加，例如：

```bash
npx skills@latest add mattpocock/skills/<skill-name>
```

将 `<skill-name>` 替换为上表中的目录名（如 `tdd`、`to-prd`）。

---

## 维护说明

- **权威指令**：代理行为以各目录 `SKILL.md` 为准；`README.zh-CN.md` 为人工阅读向摘要。
- **环境差异**：`git-guardrails`、`obsidian-vault` 等含路径或 shell 的 skill，在 Windows 或不同机器上使用前请自行核对路径与运行环境。
