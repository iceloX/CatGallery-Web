<div align="center">
  <img src="src/assets/sneezing-cat.svg" alt="Sneezing Cat" width="180" />

  <h1>喵影 · CatGallery Web</h1>

  <p>
    基于 React 19 + Ant Design 6 构建的现代化猫咪图片画廊
  </p>

  <p>
    <img src="https://img.shields.io/badge/React-19-61DAFB?logo=react" alt="React 19" />
    <img src="https://img.shields.io/badge/Ant_Design-6-1677FF?logo=antdesign" alt="Ant Design 6" />
    <img src="https://img.shields.io/badge/Vite-7-646CFF?logo=vite" alt="Vite 7" />
    <img src="https://img.shields.io/badge/License-MIT-green" alt="MIT License" />
  </p>

  <p>
    <a href="./README.md">English</a>
  </p>
</div>

---

## 关于

喵影（CatGallery Web）是一个现代化的猫咪图片画廊 Web 应用。支持用户登录认证、角色权限管理、响应式瀑布流图片浏览和管理员后台，基于 React 19、Ant Design 6 和 Vite 7 构建。

## 主要功能

- **图片画廊** — 响应式瀑布流布局，懒加载，支持相册筛选
- **用户认证** — 基于 Token 的登录，支持"记住我"
- **角色权限** — 管理员后台与普通用户视图，权限控制
- **深色 / 浅色模式** — 顶部一键切换主题
- **响应式设计** — 适配移动端，自适应任何屏幕尺寸
- **Mock 登录** — 内置开发账号，无需后端即可启动开发

## 技术栈

| 技术 | 说明 |
|------|------|
| React 19 | UI 框架（Hooks） |
| Ant Design 6 | 企业级 UI 组件库 |
| React Router 7 | 客户端路由 |
| Vite 7 | 下一代构建工具 |
| CSS Modules | 局部作用域样式 |
| Vitest | 单元测试 |

## 快速开始

```bash
# 克隆仓库
git clone https://github.com/iceloX/CatGallery-Web.git

# 安装依赖
npm install

# 启动开发服务器
npm run dev      # → http://localhost:5173

# 生产构建
npm run build

# 运行测试
npm test
```

## 开发模式 Mock 账号

开发模式内置 Mock 账号，无需配置后端：

| 账号 | 密码 | 角色 |
|------|------|------|
| admin | admin123 | 管理员 |
| user | user123 | 普通用户 |

## 项目结构

```
src/
├── views/               # 页面视图
│   ├── Index.jsx        # 首页（登录 + 画廊）
│   ├── Index.module.css
│   ├── Admin.jsx        # 管理员后台
│   └── admin/           # 管理员子页面
├── services/            # 服务层
│   ├── auth.service.js  # 认证 & Token 管理
│   ├── api.js           # API 请求封装
│   └── mock/            # Mock 数据与处理器
├── assets/              # 静态资源
│   └── sneezing-cat.svg
├── App.jsx              # 根组件（路由配置）
├── App.module.css
├── main.jsx             # 应用入口（ConfigProvider + Router）
└── style.css            # 全局样式
```

## 开源协议

本项目基于 [MIT 许可证](./LICENSE) 开源。
