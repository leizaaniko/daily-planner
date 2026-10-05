# 贡献指南

感谢你考虑为「每日工作计划 / Daily Planner」做贡献！
本文档帮助你快速了解如何参与本项目。

## 📦 项目定位

本项目坚持 **「单 HTML 文件 + 零依赖」** 的设计哲学：

- 所有 HTML、CSS、JavaScript 必须集中在 `daily-planner.html` 一个文件中
- 不引入任何 npm 依赖、外部 CDN、构建工具
- 在断网情况下双击 HTML 文件即可运行
- 数据存储仅使用浏览器原生 `localStorage`

> ⚠️ 任何引入第三方库 / 框架 / CDN 的 PR 将被拒绝。
> 如有重大架构变更想法，请先开 Issue 讨论。

## 🚀 开发流程

### 1. Fork 并克隆

```bash
git clone https://github.com/<你的用户名>/daily-planner.git
cd daily-planner
```

### 2. 创建功能分支

```bash
git checkout -b feat/your-feature
# 或修复分支
git checkout -b fix/your-bugfix
```

### 3. 本地开发

直接用浏览器打开 `daily-planner.html` 即可预览。建议使用浏览器的 DevTools：
- `Ctrl + Shift + I`（Windows / Linux）
- `Cmd + Option + I`（macOS）

### 4. 提交规范

使用 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/v1.0.0/)：

```
<type>(<scope>): <subject>

<body>

<footer>
```

常用 `type`：

| type | 说明 |
| :--- | :--- |
| `feat` | 新功能 |
| `fix` | Bug 修复 |
| `docs` | 文档变更 |
| `style` | 代码格式（不影响功能） |
| `refactor` | 重构（既不是新功能也不是修复） |
| `perf` | 性能优化 |
| `chore` | 构建 / 工具变更 |
| `revert` | 回滚 |

示例：

```
feat(task): 支持任务子任务 checklist
fix(progress): 进度环在 0 任务时显示 100% 的错误
docs(readme): 补充快捷键说明
```

### 5. 测试

本项目无自动化测试，请手动验证：

- [ ] Chrome / Edge / Firefox / Safari 主流浏览器测试通过
- [ ] 移动端响应式布局正常
- [ ] `localStorage` 数据结构 **向前兼容**（不破坏已有用户数据）
- [ ] 控制台无报错、无警告

### 6. 提交 PR

1. Push 到你 Fork 的仓库
2. 在 GitHub 上发起 Pull Request 到 `main` 分支
3. 填写 PR 模板中的检查清单
4. 等待 review

## 🐛 报告 Bug

请使用 [Bug 报告模板](https://github.com/leizaaniko/daily-planner/issues/new?template=bug_report.md) 提交 Issue，包含：

- 复现步骤
- 期望行为 vs 实际行为
- 浏览器与操作系统版本
- 控制台错误截图（如有）

## 💡 功能建议

请使用 [功能建议模板](https://github.com/leizaaniko/daily-planner/issues/new?template=feature_request.md) 提交 Issue，说明：

- 使用场景
- 期望的功能行为
- 是否有同类工具参考

## 📜 行为准则

参与本项目的所有贡献者需遵守 [行为准则](./CODE_OF_CONDUCT.md)。请保持友善、尊重、包容。

## 🏷️ Issue / PR 标签

| 标签 | 含义 |
| :--- | :--- |
| `bug` | Bug 报告 |
| `enhancement` | 功能增强 |
| `good first issue` | 适合新手的入门 Issue |
| `help wanted` | 寻求社区帮助 |
| `documentation` | 文档相关 |
| `wontfix` | 不会修复 |

## 📄 许可证

提交的代码将遵循 [MIT License](./LICENSE) 发布。
