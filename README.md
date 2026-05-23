# DeepSeek Chat Desktop

基于 Wails + Vue3 构建的 DeepSeek 桌面应用，提供便捷的桌面端访问体验。

## 功能特性

- 直接集成 `https://chat.deepseek.com/`
- 跨平台支持（Windows、macOS、Linux）
- 现代化的桌面应用体验
- 自动触发的 CI/CD 工作流

## 开发环境要求

- Go 1.21+
- Node.js 18+
- Wails v2.12+

## 快速开始

### 安装 Wails

```bash
go install github.com/wailsapp/wails/v2/cmd/wails@latest
```

### 开发模式运行

```bash
wails dev
```

### 构建应用

```bash
wails build
```

## 项目结构

```
deepseek-chat-desktop/
├── main.go                 # 主程序入口
├── app.go                  # 应用逻辑
├── wails.json              # Wails 配置
├── go.mod                  # Go 模块依赖
├── frontend/               # Vue3 前端
│   ├── src/
│   │   └── App.vue        # 主组件（嵌入 DeepSeek 聊天）
│   ├── package.json
│   └── vite.config.js
└── .github/
    └── workflows/
        └── build.yml       # GitHub Actions 工作流
```

## GitHub Actions

项目已配置 GitHub Actions 工作流，支持以下触发方式：

- **自动触发**：代码推送到 `main` 或 `master` 分支时
- **手动触发**：在 GitHub Actions 页面点击 "Run workflow"

工作流会在三个平台上构建应用：
- Ubuntu (Linux)
- Windows
- macOS

构建产物将被上传为 GitHub Actions  artifacts。

## 使用说明

1. 克隆仓库
2. 按照开发环境要求安装依赖
3. 使用 `wails dev` 进行开发
4. 或使用 `wails build` 构建生产版本

## 许可证

本项目仅供学习和个人使用。
