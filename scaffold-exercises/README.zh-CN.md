# scaffold-exercises（练习目录脚手架）

## 用途

按约定在 `exercises/` 下生成**章节 + 练习**目录结构（`XX-section`、`XX.YY-exercise`），包含 `problem/`、`solution/`、`explainer/` 等变体，并保证能通过 `pnpm ai-hero-cli internal lint`。

## 要点

- 各变体子目录需非空 `readme.md`、无坏链；有代码时还需 `main.ts` 等（见原 skill）。
- 默认 stub 可先做 `explainer/`。
- 重排目录用 `git mv` 保留历史。

## 原文

详见 [SKILL.md](./SKILL.md)。
