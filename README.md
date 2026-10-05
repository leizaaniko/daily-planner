# 每日工作计划 · Daily Planner

> 一个单文件、零依赖、即开即用的中文每日工作计划与待办事项网页应用。
> 数据保存在浏览器本地，关掉网页也不会丢失。

[![License: MIT](https://img.shields.io/github/license/leizaaniko/daily-planner?color=blue)](./LICENSE)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-success?logo=github)](https://leizaaniko.github.io/daily-planner/)
[![Last Commit](https://img.shields.io/github/last-commit/leizaaniko/daily-planner)](https://github.com/leizaaniko/daily-planner/commits/main)
[![Stars](https://img.shields.io/github/stars/leizaaniko/daily-planner?style=social)](https://github.com/leizaaniko/daily-planner/stargazers)
[![Issues](https://img.shields.io/github/issues/leizaaniko/daily-planner)](https://github.com/leizaaniko/daily-planner/issues)

---

## ✨ 功能特性

- 🎨 **现代简约深色主题**：渐变背景 + 玻璃质感卡片，视觉舒适不刺眼
- 📅 **日期与进度环**：动态问候语、当前日期 / 星期、SVG 渐变进度环直观显示完成度
- 📊 **四项统计卡片**：总任务 / 已完成 / 进行中 / 紧急，一目了然
- ✅ **任务管理**
  - 增、删、改（**双击任务标题即可编辑**）
  - 4 级优先级：紧急 / 高 / 中 / 低（左侧色条标识）
  - 4 类分类标签：工作 / 学习 / 生活 / 其他
  - 可选截止时间（24 小时制）
- 🧭 **多维度筛选**：全部 / 未完成 / 已完成 + 按分类筛选
- 💾 **localStorage 持久化**：刷新页面、关闭浏览器数据都不丢
- 📤 **导入 / 导出 JSON**：方便备份、迁移、跨设备同步
- 🗑️ **批量清理**：一键清除已完成任务、一键清空全部
- ⌨️ **键盘快捷键**：`N` 新建、`A` 全部、`U` 未完成、`Enter` 提交
- 📱 **响应式布局**：桌面、平板、手机均适配
- 🌐 **零依赖**：单 HTML 文件 + 原生 JavaScript，无需构建、无需服务器

## 🚀 快速开始

### 方式一：在线使用（推荐）

直接访问 GitHub Pages 部署：

> **https://leizaaniko.github.io/daily-planner/**

建议添加到浏览器书签作为每日工具。

### 方式二：本地使用

1. 克隆仓库
   ```bash
   git clone https://github.com/leizaaniko/daily-planner.git
   ```
2. 双击 `daily-planner.html` 用任意现代浏览器打开即可

### 方式三：直接下载单文件

从 [Releases](https://github.com/leizaaniko/daily-planner/releases) 下载 `daily-planner.html`，无需克隆整个仓库。

## ⌨️ 键盘快捷键

| 快捷键 | 功能 |
| :---: | :--- |
| `N` | 聚焦到任务输入框，开始添加新任务 |
| `A` | 切换到「全部」筛选 |
| `U` | 切换到「未完成」筛选 |
| `Enter` | 在输入框中按 Enter 提交任务 |
| 双击标题 | 进入编辑模式 |
| `Esc` | 编辑时按 Esc 取消修改 |

## 🔒 数据与隐私

- ✅ 所有任务数据存储在浏览器的 `localStorage` 中
- ✅ 不上传任何数据到服务器，无追踪、无账号
- ⚠️ **跨设备不同步**：每个浏览器、每台设备的数据相互独立
- 💡 如需跨设备迁移：使用「导出 JSON」备份，在另一台设备「导入 JSON」

存储键名：`daily-planner-tasks-v1`。如需重置应用，可在浏览器开发者工具中清除该键。

## 🛠️ 技术栈

| 类别 | 选型 |
| :--- | :--- |
| 结构 | 原生 HTML5 |
| 样式 | 原生 CSS3 + CSS 变量 + Flexbox / Grid |
| 交互 | 原生 JavaScript（ES6+，无框架、无构建） |
| 持久化 | `localStorage` Web API |
| 进度可视化 | SVG + `stroke-dashoffset` 动画 |
| 字体 | 系统字体栈（PingFang SC / Microsoft YaHei 等） |

## 📁 项目结构

```
daily-planner/
├── daily-planner.html        # 主应用文件（HTML + CSS + JS 单文件）
├── README.md                 # 项目说明文档
├── LICENSE                   # MIT 开源协议
├── CHANGELOG.md              # 版本变更日志
├── CONTRIBUTING.md           # 贡献指南
├── CODE_OF_CONDUCT.md        # 行为准则
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── bug_report.md     # Bug 报告模板
    │   └── feature_request.md # 功能建议模板
    └── PULL_REQUEST_TEMPLATE.md # PR 模板
```

## 🎯 自定义

由于是单 HTML 文件，所有样式都在 `<style>` 标签内的 `:root` 变量中，**修改 CSS 变量即可整体换肤**：

```css
:root {
  --bg: #0b1020;          /* 主背景 */
  --surface: #1e293b;     /* 卡片背景 */
  --accent: #60a5fa;      /* 强调色 */
  --urgent: #ef4444;      /* 紧急优先级色 */
  --high: #f97316;        /* 高优先级色 */
  --medium: #eab308;      /* 中优先级色 */
  --low: #22c55e;         /* 低优先级色 */
  /* …其他变量见文件头部 */
}
```

## 🗺️ 路线图

- [ ] 浅色 / 深色双主题切换
- [ ] 任务子任务（checklist）
- [ ] 每周 / 每月统计视图
- [ ] i18n 中英双语切换
- [ ] PWA 离线支持（manifest + service worker）
- [ ] 提醒通知（Web Notifications API）
- [ ] 数据云端同步（可选）

详见 [Issues](https://github.com/leizaaniko/daily-planner/issues) 中的 `enhancement` 标签。欢迎提出新想法。

## 🤝 贡献

欢迎提交 Issue、Pull Request 或 Star 支持。请先阅读：

- [贡献指南](./CONTRIBUTING.md)
- [行为准则](./CODE_OF_CONDUCT.md)

提交 PR 前请确保：
1. 功能在主流浏览器（Chrome / Edge / Firefox / Safari）测试通过
2. 不引入第三方依赖（保持「单文件零依赖」的设计哲学）
3. `localStorage` 数据结构向前兼容（不破坏已有用户数据）

## 📄 许可证

[MIT License](./LICENSE) © 2026 [leizaaniko](https://github.com/leizaaniko)

可自由使用、修改、分发、商用，但请保留原作者许可声明。

## 🙏 致谢与参考

本项目在设计思路上参考了以下优秀的开源项目 / 文章：

- [TaskFlow](https://dev.to/mou1z/build-a-todoist-alternative-with-500-lines-of-vanilla-javascript-14pa) — 单文件 todo 管理器，状态驱动渲染思路
- [Daily TODO](https://github.com/minhajuddin/dailytodo) — 按星期过滤任务的设计
- [1-3-5 List](https://github.com/neely/apps/blob/main/135-todo.html) — 静态 HTML + localStorage 的极简思路

感谢 [GitHub CLI](https://cli.github.com/) 让仓库初始化如此顺滑。

## 📞 联系

- Issue：[github.com/leizaaniko/daily-planner/issues](https://github.com/leizaaniko/daily-planner/issues)
- 作者：[@leizaaniko](https://github.com/leizaaniko)

如果这个项目对你有帮助，欢迎 ⭐ Star 让更多人看到。
