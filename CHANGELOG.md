# 变更日志

本项目遵循 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.1.0/) 规范，
版本号遵循 [Semantic Versioning](https://semver.org/lang/zh-CN/)。

## [Unreleased]

### 计划中
- 浅色 / 深色双主题切换
- 任务子任务（checklist）
- 每周 / 每月统计视图
- i18n 中英双语切换
- PWA 离线支持

## [1.0.0] - 2026-10-05

### 新增
- ✨ 初始版本发布
- 🎨 现代简约深色主题，渐变背景 + 玻璃质感卡片
- 📅 日期卡片：动态问候语、当前日期 / 星期、SVG 渐变进度环
- 📊 四项统计卡片：总任务 / 已完成 / 进行中 / 紧急
- ✅ 任务管理：
  - 添加、删除、双击标题编辑
  - 4 级优先级（紧急 / 高 / 中 / 低），左侧色条标识
  - 4 类分类标签（工作 / 学习 / 生活 / 其他）
  - 可选截止时间（24 小时制）
- 🧭 多维度筛选：全部 / 未完成 / 已完成 + 按分类筛选
- 💾 localStorage 持久化，键名 `daily-planner-tasks-v1`
- 📤 导入 / 导出 JSON（备份、迁移、跨设备同步）
- 🗑️ 批量清理：清除已完成、清空全部
- ⌨️ 键盘快捷键：`N` 新建、`A` 全部、`U` 未完成、`Enter` 提交
- 📱 响应式布局，桌面 / 平板 / 手机适配
- 🌐 单 HTML 文件 + 原生 JavaScript，零依赖
- 🌸 首次访问 4 条示例任务引导
- 📦 GitHub Pages 部署：https://leizaaniko.github.io/daily-planner/

### 文档
- 完整 README.md（功能、使用、快捷键、技术栈、自定义、路线图）
- MIT LICENSE
- CONTRIBUTING.md 贡献指南
- CODE_OF_CONDUCT.md 行为准则
- GitHub Issue 模板（bug 报告、功能建议）
- GitHub Pull Request 模板

[Unreleased]: https://github.com/leizaaniko/daily-planner/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/leizaaniko/daily-planner/releases/tag/v1.0.0
