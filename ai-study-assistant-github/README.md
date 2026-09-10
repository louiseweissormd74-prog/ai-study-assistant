# AI 学习助手

一个基于 HTML、Tailwind CSS 与原生 JavaScript 构建的响应式 AI 学习工作台原型。

## 功能

- AI 作业助手、PDF 智能总结、课堂转录、数学分步解题与论文写作助手
- 学习工具快速切换、Prompt 一键填充与文件选择反馈
- 模拟 AI 结构化回答、复制、评价与重新生成操作
- 学习目标、学习节奏、最近记录与通知中心
- 桌面端与移动端响应式布局

## 本地预览

直接打开 `dist/index.html`，或在项目根目录启动任意静态文件服务器并将目录指向 `dist`。

例如：

```bash
npx serve dist
```

## 部署到 GitHub Pages

1. 在 GitHub 新建一个空仓库。
2. 将本项目全部文件上传到仓库的 `main` 分支。
3. 打开仓库的 **Settings → Pages**。
4. 在 **Build and deployment** 中，将 Source 选择为 **GitHub Actions**。
5. 打开仓库的 **Actions** 页面，等待 `Deploy AI Study Assistant to GitHub Pages` 执行完成。

部署地址通常为：

```text
https://你的用户名.github.io/仓库名/
```

页面使用相对路径并包含 `.nojekyll`，可直接部署到用户主页或项目子路径。

## 项目结构

```text
.
├── .github/
│   └── workflows/
│       └── deploy-pages.yml
├── dist/
│   ├── .nojekyll
│   └── index.html
└── README.md
```

## 技术说明

- Tailwind CSS 通过官方浏览器 CDN 加载。
- 图标使用 Lucide UMD CDN。
- 不依赖后端服务或密钥；AI 回答为前端交互演示。
