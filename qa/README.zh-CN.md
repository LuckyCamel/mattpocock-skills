# qa（交互式 QA 与建 Issue）

## 用途

用户口语描述遇到的问题；代理**轻度澄清**（最多 2～3 个短问题），后台用 Explore 子代理扫代码以掌握**领域用语与行为边界**，然后用 **`glab issue create`** **直接**创建 GitLab Issue（不先让用户审稿），适合「边聊边报 bug / 开单」。

## Issue 写作原则

- **面向行为、面向用户**：不写具体文件路径与行号（易过期）。
- 使用项目领域语言（若有 `UBIQUITOUS_LANGUAGE.md` 应对齐）。
- 判断是**单 issue** 还是拆成多个可并行、有依赖关系的薄 issue。
- 使用 skill 内模板：`What happened` / `Expected` / `Steps` / `Additional context` 等。

## 原文

详见 [SKILL.md](./SKILL.md)。
