# migrate-to-shoehorn（测试数据：as → shoehorn）

## 用途

把测试里的 TypeScript `as` 断言迁移到 `@total-typescript/shoehorn`，用类型安全方式构造**部分**或**故意错误**的测试数据。仅用于**测试代码**，生产代码不要用 shoehorn。

## 常见映射

- `as Type` → `fromPartial(...)`
- `as unknown as Type`（故意类型错误）→ `fromAny(...)`
- 另有 `fromExact()` 等，见原 skill 表格。

## 工作流概要

1. 与用户确认要改的测试文件、`as` 使用场景（大对象只关心少数字段、是否要测错误类型等）。
2. 安装包：`npm i @total-typescript/shoehorn`（需本地自行安装）。
3. 搜索测试中的 `as`，替换并跑类型检查。

## 原文

详见 [SKILL.md](./SKILL.md)。
