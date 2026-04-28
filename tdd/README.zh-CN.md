# tdd（测试驱动开发）

## 用途

按 **红—绿—重构** 循环，用**竖切（vertical slice）**一次只加一个测试与刚好通过的实现；强调通过**公开接口**验证行为，避免实现细节耦合。适用于功能开发、修 bug、或用户明确要 TDD / red-green-refactor。

## 核心原则

- **禁止横切**：不要先写一堆测试再写一堆实现（会产生脆弱、脱离真实行为的测试）。
- **Tracer bullet**：先一个端到端行为测试 → 最小实现通过 → 再下一个。
- **重构只在全绿后**；更多见同目录 [tests.md](./tests.md)、[mocking.md](./mocking.md)、[deep-modules.md](./deep-modules.md) 等。

## 原文

详见 [SKILL.md](./SKILL.md)。
