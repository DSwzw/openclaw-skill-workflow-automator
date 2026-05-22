# Workflow Automator ⚙️

> OpenClaw-native 工作流自动化引擎 — 用简化 YAML 定义多步骤任务管道，支持日志、重试、条件分支和定时调度。

## 安装

```bash
# 通过 SkillHub
skillhub install workflow-automator

# 或手动
git clone https://github.com/qifengle-ovo/openclaw-skill-workflow-automator.git
```

## 使用场景

- 定义可重复的多步骤任务管道（备份、部署、监控、报告）
- 通过 cron 定时调度工作流
- 顺序执行命令并记录日志和错误
- 管理工作流执行历史和状态
- 导出工作流分享给团队

## 快速开始

```bash
# 创建新工作流
workflow create backup --template daily-backup

# 运行工作流
workflow run backup

# 查看状态
workflow status

# 定时调度
workflow schedule backup --cron "0 2 * * *"
```

## 核心特性

- ✅ 零依赖 — 纯 Bash 实现
- ✅ 轻量级 — 比 Python/Node.js 方案更轻
- ✅ 容错 — 内置重试和错误处理
- ✅ 条件分支 — if/then/else 支持
- ✅ 日志追踪 — 完整执行记录

## 文档

详见 [SKILL.md](./SKILL.md)

## License

MIT-0