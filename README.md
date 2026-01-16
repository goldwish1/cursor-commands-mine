# Cursor Commands

⭐ **由 [Cursor](https://x.com/ericzakariasson/status/1973932448200413539) 推荐**

一个精选的 Cursor 斜杠命令提示词集合，为您的团队提供可在 Cursor IDE 中直接使用的可复用、版本控制的 AI 工作流。

🔗 同时查看 [Cursor Hooks](https://github.com/hamzafer/cursor-hooks) - 在每次文件编辑后运行

## 什么是 Cursor Commands？

Cursor Commands 是可复用的 AI 提示词，以 Markdown 文件形式保存在 `.cursor/commands/` 目录中。当您在 Cursor 的聊天输入框中输入 `/` 时，IDE 会列出项目中和全局库中的每个命令，以便您立即插入提示词。它们就像 AI 驱动的快捷方式，可以自动化重复性任务，强化团队标准，并保持反馈的一致性。

## 功能特性

- **🚀 快速访问**：输入 `/` 即可显示所有命令，无需离开您的工作流程
- **🔄 可复用**：为整个团队的常见任务标准化提示词
- **👥 可共享**：将命令存储在 git 中，以便它们随您的仓库一起发布
- **🎯 聚焦**：每个命令都针对具有清晰结构的特定工作流
- **📝 可定制**：编辑或扩展 Markdown 文件以匹配您的流程

## 命令的工作原理

命令可以存在于两个位置：

- **项目命令**：在仓库内的 `.cursor/commands` 中存储 Markdown 文件
- **全局命令**：在您机器上的 `~/.cursor/commands` 中存储个人命令

当您输入 `/` 时，Cursor 会自动扫描这两个目录，合并结果，并将选定的命令插入到聊天中，准备运行。

## 如何使用

1. 在 Cursor 的 AI 聊天或代理输入框中输入 `/`
2. 从可用命令中选择
3. 让 AI 在相关的项目上下文中执行提示词

## 创建命令

- 在项目根目录创建 `.cursor/commands` 目录
- 添加具有描述性名称的 `.md` 文件（例如，`code-review.md`、`run-all-tests-and-fix.md`）
- 编写清晰的 Markdown 说明，描述命令应完成的任务
- 打开 Cursor，输入 `/`，选择您的新命令即可立即执行

示例结构：

```text
.cursor/
└── commands/
    ├── accessibility-audit.md
    ├── add-documentation.md
    ├── add-error-handling.md
    ├── address-github-pr-comments.md
    ├── clarify-task.md
    ├── code-review.md
    ├── create-pr.md
    ├── deslop.md
    ├── docker-logs.md
    ├── database-migration.md
    ├── debug-issue.md
    ├── diagrams.md
    ├── fix-compile-errors.md
    ├── fix-git-issues.md
    ├── generate-api-docs.md
    ├── generate-pr-description.md
    ├── git-commit.md
    ├── git-push.md
    ├── light-review-existing-diffs.md
    ├── lint-fix.md
    ├── lint-suite.md
    ├── onboard-new-developer.md
    ├── optimize-performance.md
    ├── overview.md
    ├── refactor-code.md
    ├── roadmap.md
    ├── run-all-tests-and-fix.md
    ├── security-audit.md
    ├── security-review.md
    ├── setup-new-feature.md
    ├── visualize.md
    └── write-unit-tests.md
```

## 可用命令

### 代码质量与维护

- `lint-fix.md` – 自动分析并修复当前文件中的 linting 问题
- `lint-suite.md` – 运行项目 linter，应用修复，确保代码库满足格式要求
- `refactor-code.md` – 在保持功能的同时提高代码质量
- `optimize-performance.md` – 分析并优化代码性能
- `add-error-handling.md` – 在整个变更集中实现全面的错误处理
- `deslop.md` – 通过移除不必要的复杂性和冗余来清理 AI 生成的代码
- `clarify-task.md` – 将模糊的任务分解为清晰、可操作的步骤

### 审查与协作

- `code-review.md` – 具有结构化步骤和重点领域的全面审查清单
- `address-github-pr-comments.md` – 处理审查者反馈并制定周到的回复
- `light-review-existing-diffs.md` – 快速检查以突出显示有风险的差异和清理项
- `create-pr.md` – 准备结构良好的拉取请求，包含验证清单
- `generate-pr-description.md` – 自动生成详细的拉取请求描述

### 测试与可靠性

- `run-all-tests-and-fix.md` – 执行完整测试套件，分类失败并确认修复
- `write-unit-tests.md` – 生成具有适当覆盖率的聚焦单元测试
- `debug-issue.md` – 用于隔离缺陷的分步调试工作流
- `fix-compile-errors.md` – 快速诊断并解决编译失败
- `docker-logs.md` – 跟踪和监控 Docker 容器日志以进行调试

### 文档与入职

- `add-documentation.md` – 捕获全面的产品或代码文档
- `generate-api-docs.md` – 生成包含模式和示例的丰富 API 文档
- `onboard-new-developer.md` – 为新队友提供清单驱动的入职流程
- `setup-new-feature.md` – 为新工作规划需求、分支和架构
- `visualize.md` – 从代码或概念生成可视化图表和流程图
- `diagrams.md` – 生成 Mermaid 图表（流程图、序列图、类图、ER 图、状态图）
- `overview.md` – 为用户旅程和架构流程生成 Mermaid 图表
- `roadmap.md` – 分析代码库并生成可视化功能路线图

### 安全性、可访问性与基础设施

- `security-audit.md` – 用于代码变更的结构化安全检查清单
- `security-review.md` – 更广泛的漏洞和风险评估工作流
- `accessibility-audit.md` – 审查 WCAG 合规性问题
- `database-migration.md` – 规划、创建和验证数据库迁移，包含回滚
- `fix-git-issues.md` – 安全地解决合并冲突和仓库问题

### Git 工作流

- `git-commit.md` – 创建结构良好的提交消息，可选择链接问题键
- `git-push.md` – 在推送前检查后将更改推送到远程

## 快速开始

1. 克隆此仓库或将 `.cursor/commands/` 目录复制到您的项目中
2. 在 Cursor IDE 中打开项目
3. 在 AI 聊天中输入 `/` 以浏览可用命令
4. 选择一个命令，让 Cursor 在您的代码上下文中执行提示词

## 安装选项

```bash
# 选项 1：克隆仓库
git clone https://github.com/hamzafer/cursor-commands.git
cd cursor-commands
```

```bash
# 选项 2：将命令复制到现有项目中
cp -r cursor-commands/.cursor /path/to/your/project/
```

或者，手动创建目录：

1. 在项目根目录创建 `.cursor/commands/`
2. 复制或编写您需要的 Markdown 命令文件

## 编写您自己的命令

使用现有文件作为模板或从头开始：

```bash
touch .cursor/commands/my-custom-command.md
```

```markdown
# 我的自定义命令

简要描述此命令的作用。

## 目标
详细说明任务和预期结果。

## 要求
- 特定要求或约束
- 要遵循的编码标准
- 预期格式或结构

## 输出
描述 AI 应产生的内容。

为 AI 提供清晰的说明。
```

## 示例提示词

```markdown
# 生成 API 文档

为当前代码创建全面的 API 文档。包括：

- 端点描述和 HTTP 方法
- 带有示例的请求/响应模式
- 身份验证要求
- 错误代码和响应
- 速率限制信息

格式化为 OpenAPI/Swagger 规范。
```

```markdown
# 安全审计

对当前代码执行安全审计。检查：

- SQL 注入漏洞
- XSS 攻击向量
- 身份验证和授权问题
- 输入验证问题
- 敏感数据暴露

为发现的每个问题提供具体的修复步骤。
```

## 最佳实践

- **具体明确**：描述预期结果和验收标准
- **提供上下文**：参考项目约定、架构或标准
- **设定边界**：明确范围、假设和工具限制
- **包含示例**：在有用时显示预期格式或响应
- **保持专注**：让每个命令都针对单一、清晰的目标
- **共同审查**：将命令更改视为代码更改，在 PR 中审查
- **使用描述性名称**：使文件名反映命令的用途

## 参考资料

- [更新日志 – v1.6](https://cursor.com/changelog)
- [文档 – 自定义斜杠命令](https://cursor.com/docs/agent/chat/commands)
- [公告帖子 1](https://x.com/cursor_ai/status/1967990959645528195)
- [公告帖子 2](https://x.com/cursor_ai/status/1970185277923615188)

## 支持

- 打开 [issue](https://github.com/hamzafer/cursor-commands/issues) 提供反馈或请求
- 参考此 README 了解随提示词一起提供的命令索引

## 许可证

此项目是开源的，可在 [MIT 许可证](LICENSE) 下使用。
