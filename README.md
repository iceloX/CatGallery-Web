<div align="center">
  <img src="src/assets/sneezing-cat.svg" alt="Sneezing Cat" width="180" />

  <h1>CatGallery Web · 喵影</h1>

  <p>
    A modern cat photo gallery built with React 19 + Ant Design 6
  </p>

  <p>
    <img src="https://img.shields.io/badge/React-19-61DAFB?logo=react" alt="React 19" />
    <img src="https://img.shields.io/badge/Ant_Design-6-1677FF?logo=antdesign" alt="Ant Design 6" />
    <img src="https://img.shields.io/badge/Vite-7-646CFF?logo=vite" alt="Vite 7" />
    <img src="https://img.shields.io/badge/License-MIT-green" alt="MIT License" />
  </p>

  <p>
    <a href="./README.zh-CN.md">简体中文</a>
  </p>
</div>

---

## About

CatGallery Web (喵影) is a modern web application for browsing and managing cat photos. It features user authentication, role-based access control, a responsive waterfall-layout photo gallery, and an admin dashboard — all built with React 19, Ant Design 6, and Vite 7.

## Features

- **Photo Gallery** — Responsive waterfall layout with lazy loading and album filtering
- **Authentication** — Token-based login with "Remember Me" support
- **Role-based Access** — Admin dashboard and user views with permission control
- **Dark / Light Mode** — One-click theme toggle in the header
- **Responsive Design** — Mobile-friendly, adapts to any screen size
- **Mock Login** — Built-in dev accounts, no backend required to get started

## Tech Stack

| Technology | Description |
|-----------|-------------|
| React 19 | UI framework with Hooks |
| Ant Design 6 | Enterprise-grade UI components |
| React Router 7 | Client-side routing |
| Vite 7 | Next-gen build tool |
| CSS Modules | Scoped styling |
| Vitest | Unit testing |

## Quick Start

```bash
# Clone the repository
git clone https://github.com/iceloX/CatGallery-Web.git

# Install dependencies
npm install

# Start dev server
npm run dev      # → http://localhost:5173

# Production build
npm run build

# Run tests
npm test
```

## Mock Accounts

Dev mode includes built-in mock accounts (no backend needed):

| Account | Password | Role |
|---------|----------|------|
| admin | admin123 | Admin |
| user | user123 | User |

## Project Structure

```
src/
├── views/               # Page views
│   ├── Index.jsx        # Homepage (login + gallery)
│   ├── Index.module.css
│   ├── Admin.jsx        # Admin dashboard
│   └── admin/           # Admin sub-pages
├── services/            # Service layer
│   ├── auth.service.js  # Auth & token management
│   ├── api.js           # API request wrapper
│   └── mock/            # Mock data & handlers
├── assets/              # Static assets
│   └── sneezing-cat.svg
├── App.jsx              # Root component (routes)
├── App.module.css
├── main.jsx             # App entry (ConfigProvider + Router)
└── style.css            # Global styles
```

## License

This project is open sourced under the [MIT License](./LICENSE).
