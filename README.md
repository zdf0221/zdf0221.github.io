# ClawServe 钳瑟夫

<p align="center">
  <img src="https://via.placeholder.com/120x120/FF6B6B/FFFFFF?text=CS" alt="ClawServe Logo" width="120" />
</p>

<p align="center">
  <strong>基于 OpenClaw 的智能服务专家</strong><br>
  部署 · 托管 · 运维 · 一站式解决方案
</p>

<p align="center">
  <a href="#功能特性">功能特性</a> •
  <a href="#技术栈">技术栈</a> •
  <a href="#本地预览">本地预览</a> •
  <a href="#部署">部署</a> •
  <a href="#项目结构">项目结构</a>
</p>

---

## 📖 项目介绍

**ClawServe 钳瑟夫**是一个专注于 OpenClaw 生态的技术服务平台，致力于为企业级用户提供：

- **智能部署**：快速部署 OpenClaw 环境，一键启动
- **稳定托管**：7×24小时云端托管，高可用保障
- **专业运维**：监控、备份、升级全包服务

> **OpenClaw** 是一个开源的多 Agent 协作框架，支持 AI Agent 之间的任务分发、协调与监控。

## ✨ 功能特性

### 🎯 核心功能

| 功能模块 | 描述 |
|---------|------|
| **响应式官网** | 适配桌面端、平板、手机等多种设备 |
| **服务展示** | 清晰展示三大核心服务能力 |
| **价格方案** | 三档定价（Starter/Professional/Enterprise） |
| **技术咨询** | OpenClaw 多 Agent 架构设计咨询 |
| **联系表单** | Modal 弹窗式咨询表单，支持套餐选择 |

### 🎨 设计亮点

- **海洋主题配色**：深海蓝 + 龙虾红/珊瑚橙的渐变设计
- **龙虾吉祥物**：SVG 绘制的品牌吉祥物
- **波浪动效**：Hero 区域的波浪分割和浮动动画
- **币种切换**：支持 CNY/USD 实时切换

## 🛠️ 技术栈

### 前端技术
- **HTML5** - 语义化页面结构
- **Tailwind CSS** - 实用优先的 CSS 框架（CDN 引入）
- **Font Awesome** - 图标库（CDN 引入）
- **Google Fonts** - Inter + Noto Sans SC 字体

### 开发工具
- **VS Code** - 代码编辑器
- **Live Server** - 本地开发服务器

## 📁 项目结构

```
clawserve-website/
├── index.html          # 主页面（完整 SPA）
├── css/
│   └── style.css       # 自定义样式（龙虾主题）
├── js/
│   └── app.js          # 交互逻辑（导航、Modal、动画）
├── images/             # 图片资源目录
└── README.md           # 本文件
```

### 关键文件说明

| 文件 | 说明 |
|------|------|
| `index.html` | 单页应用主文件，包含所有区块（Hero/服务/价格/支持/Footer） |
| `css/style.css` | 自定义样式：龙虾主题配色、动画效果、响应式断点 |
| `js/app.js` | 交互逻辑：导航滚动效果、Modal、币种切换、平滑滚动 |

## 🚀 本地预览

### 方式一：Python 简单服务器

```bash
cd clawserve-website
python3 -m http.server 8080

# 浏览器访问
open http://localhost:8080
```

### 方式二：Node.js http-server

```bash
# 安装 http-server
npm install -g http-server

# 启动服务
cd clawserve-website
http-server -p 8080

# 浏览器访问
open http://localhost:8080
```

### 方式三：VS Code Live Server

1. 安装 VS Code 插件 **Live Server**
2. 右键点击 `index.html`
3. 选择 "Open with Live Server"

## 🌐 部署

### GitHub Pages 部署

1. **Fork 或创建仓库**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/username/clawserve-website.git
   git push -u origin main
   ```

2. **启用 GitHub Pages**
   - 进入仓库 Settings → Pages
   - Source 选择 "Deploy from a branch"
   - Branch 选择 `main` / `root`
   - 点击 Save

3. **访问网站**
   - 等待几分钟后访问 `https://username.github.io/clawserve-website`

### 其他部署方式

- **Vercel**: 直接导入 Git 仓库自动部署
- **Netlify**: 拖拽上传或连接 Git 仓库
- **Cloudflare Pages**: 原生支持静态网站

## 📱 响应式断点

| 断点 | 宽度 | 布局调整 |
|------|------|---------|
| Desktop | > 1024px | 三列价格卡片，完整导航 |
| Tablet | 768px - 1024px | 两列布局，适配触控 |
| Mobile | < 768px | 单列布局，汉堡菜单 |

## 🎨 品牌配色

| 颜色名称 | 色值 | 用途 |
|---------|------|------|
| 深海蓝 | `#0A2540` | 主色调、导航、Footer |
| 龙虾红 | `#FF6B6B` | CTA按钮、强调色 |
| 珊瑚橙 | `#FF8C42` | 渐变、悬停状态 |
| 金色 | `#FFD700` | "最受欢迎"标签 |
| 浅灰 | `#F7FAFC` | 背景色 |

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

### 提交规范

- 使用清晰的 commit message
- 保持代码风格一致
- 测试响应式效果
- 不引入外部依赖（CDN 除外）

## 📄 许可证

本项目采用 [MIT License](LICENSE) 开源协议。

```
MIT License

Copyright (c) 2026 ClawServe

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

## 📞 联系方式

- **邮箱**: hello@clawserve.com
- **官网**: https://clawserve.com
- **技术支持**: 详见网站内"技术支持"板块

---

<p align="center">
  Made with ❤️ by the ClawServe Team
</p>
