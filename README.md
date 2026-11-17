# tell-me-first

`tell-me-first` 是一个 Codex Skill，将开发任务分为需求对齐、目标和方案确认、实施开发并总结、测试并生成报告四个步骤。每个阶段根据用户确认推进，适用于功能开发、问题修复和重构。

## 安装

将本项目中的整个 `tell-me-first` 目录复制到 Codex 的 skills 目录，例如：

```bash
cp -R tell-me-first ~/.codex/skills/
```

请保留 `references/` 目录，入口需要从中读取各步骤和方案模板。

## 使用

在 Codex 中调用 `$tell-me-first` 并说明任务。Skill 会先对齐需求，再根据用户确认逐步推进方案、实施和测试。用户可以明确授权具体方案及测试安排。

## 项目结构

```text
tell-me-first/
├── SKILL.md                       # 入口及步骤衔接
└── references/
    ├── develop-step-1-align.md    # 需求对齐
    ├── develop-step-2-scope.md    # 目标和方案确认
    ├── develop-step-3-implement.md # 实施开发并总结
    ├── develop-step-4-test.md     # 测试并生成报告
    └── scope-proposal.md          # 方案模板
```

## 许可证

[MIT](LICENSE)
