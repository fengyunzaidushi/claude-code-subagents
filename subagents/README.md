# Claude Code Subagents 子智能体

本仓库包含按功能域分类的 Claude Code 子智能体，基于 [Claude Code 官方文档](https://docs.anthropic.com/en/docs/claude-code/sub-agents) 重新组织。

## 目录结构

### 🏗️ Architecture (架构)
专注于系统设计和架构决策的子智能体：
- `architect-review.md` - 架构审查专家
- `backend-architect.md` - 后端架构师
- `cloud-architect.md` - 云架构师  
- `graphql-architect.md` - GraphQL 架构师

### 💻 Development (开发)
专注于特定技术栈开发的子智能体：
- `ai-engineer.md` - AI 工程师
- `frontend-developer.md` - 前端开发者
- `go-developer.md` - Go 开发者
- `mobile-developer.md` - 移动开发者
- `python-developer.md` - Python 开发者

### 🚀 Operations (运维)
专注于部署、运维和性能优化的子智能体：
- `database-optimizer.md` - 数据库优化师
- `deployment-engineer.md` - 部署工程师
- `devops-troubleshooter.md` - DevOps 故障排除专家
- `incident-responder.md` - 事件响应专家
- `performance-engineer.md` - 性能工程师

### 🔒 Security (安全)
专注于安全审计和防护的子智能体：
- `security-auditor.md` - 安全审计员
- `security-scanner/` - 安全扫描器

### ✅ Quality Assurance (质量保证)
专注于代码质量、测试和重构的子智能体：
- `code-reviewer.md` - 代码审查员
- `code-reviewer/` - 代码审查器目录
- `debugger.md` - 调试专家
- `debugger/` - 调试器目录
- `refactor/` - 重构专家目录
- `test-automator.md` - 测试自动化专家
- `test-runner/` - 测试运行器目录

### 📊 Data Science (数据科学)
专注于数据处理和机器学习的子智能体：
- `data-engineer.md` - 数据工程师
- `data-scientist.md` - 数据科学家
- `ml-engineer.md` - 机器学习工程师
- `quant-analyst.md` - 量化分析师

### 🔧 Specialized (专业化)
专注于特定领域或任务的子智能体：
- `api-documenter.md` - API 文档编写专家
- `context-manager.md` - 上下文管理器
- `developer-experience.md` - 开发者体验优化师
- `doc-writer/` - 文档编写器目录
- `legacy-modernizer.md` - 遗留系统现代化专家
- `payment-integration.md` - 支付集成专家
- `prompt-engineer.md` - 提示工程师

## 使用方法

### 项目级别使用
将所需的子智能体复制到项目的 `.claude/agents/` 目录：
```bash
cp subagents/development/frontend-developer.md .claude/agents/
```

### 用户级别使用
将子智能体复制到用户目录：
```bash
cp subagents/quality-assurance/code-reviewer.md ~/.claude/agents/
```

## 子智能体结构

每个子智能体都包含：
- **name**: 唯一标识符（小写，连字符分隔）
- **description**: 子智能体的用途和触发条件
- **系统提示**: 详细的角色定义和工作方式

## 最佳实践

1. **专一职责**: 每个子智能体专注于特定领域
2. **清晰命名**: 使用描述性的名称和分类
3. **适当工具**: 根据需要限制工具访问权限
4. **版本控制**: 将项目级子智能体纳入版本控制

## 贡献指南

添加新子智能体时，请：
1. 选择合适的分类目录
2. 使用一致的命名约定
3. 包含完整的 YAML 前置元数据
4. 编写清晰的系统提示
5. 更新本 README 文件

---

基于 Claude Code 官方文档重新组织，提供更好的结构化和可维护性。