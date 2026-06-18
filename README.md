# coding-instructions

> Andrej Karpathy 编程准则 + Gitmoji 提交与分支工作流规范

一套面向 AI 辅助编程的极简主义工作流规范，帮助个人与小团队在借助 AI 写代码时保持代码简洁、提交历史清晰、合并流程可控。

## 特性

- **极简主义编码**：从最短、自包含、零依赖的实现开始，逐步增加复杂度。
- **先复制，再创新**：优先复用成熟方案，一次只引入一个复杂度。
- **理解底层原理**：避免黑盒调用，代码体现对底层机制的理解。
- **功能分支开发**：所有新功能、修复、文档改动都在独立分支上完成。
- **Gitmoji 提交规范**：使用直观的 emoji 前缀，让提交意图一目了然。
- **测试通过后合并**：合并前必须完成测试并请求许可，禁止自行合并。

## 使用方式

1. 将 `coding-instructions.md` 放入你的 Kimi Code skill 目录（例如 `.kimi-code/skills/`）。
2. 在需要遵循该规范的会话中激活 skill。
3. AI 代理将在编码、提交、分支与合并过程中自动遵循本规范。

## 规范摘要

### 编码原则

1. 极简主义 — 从简开始
2. "不要做英雄" — 先复制，再创新
3. 理解底层原理
4. 从简单到复杂 — 循序渐进
5. 简洁代码风格
6. 最小依赖

### Git 工作流

- 新功能基于 `feature/<描述>`、`fix/<描述>`、`docs/<描述>` 等功能分支开发。
- 每完成一个逻辑步骤就提交一次，提交格式：`<emoji> <type>: <描述>`。
- 合并前运行完整测试，向维护者请求合并许可。
- 合并一律使用 `git merge` 或 squash merge，禁止用 rebase 替代 merge。
- 合并后删除已合并的分支。

完整规范请查看 [`coding-instructions.md`](./coding-instructions.md)。

## 文件说明

| 文件 | 说明 |
|------|------|
| `coding-instructions.md` | 完整的编程与 Git 工作流规范 |
| `README.md` | 项目简介与使用指南 |
| `CONTRIBUTING.md` | 贡献指南 |
| `LICENSE` | 开源许可证 |
| `.gitignore` | Git 忽略规则 |

## 贡献

欢迎通过 Issue 或 Pull Request 提出改进建议。请先阅读 [`CONTRIBUTING.md`](./CONTRIBUTING.md)。

## 许可证

本项目采用 [MIT 许可证](./LICENSE)。
