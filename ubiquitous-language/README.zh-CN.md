# ubiquitous-language（通用语言词汇表）

## 用途

从**当前对话**抽取领域名词、动词与概念，识别同词异义、同义多词与模糊用语，给出**带观点的规范术语表**，写入工作目录下的 **`UBIQUITOUS_LANGUAGE.md`**，并在对话里输出摘要。适合统一术语、DDD 式词汇、或用户提到 ubiquitous language。

## 输出结构要点

- 按主题分组的表格：Term / Definition / Aliases to avoid。
- **Relationships**：概念之间关系与基数。
- **Example dialogue**：3～5 轮 dev 与领域专家对话，示范术语如何精确使用。
- **Flagged ambiguities**：明确写出冲突与建议。
- 跳过纯编程通用词，除非在域内有特殊含义。

## 再次运行

会读取已有文件并合并新讨论、更新定义与示例对话。

## 原文

详见 [SKILL.md](./SKILL.md)。
