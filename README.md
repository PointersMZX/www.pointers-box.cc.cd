# Pointers-BOX 官方网站

本仓库是 Pointers-BOX 官方网站 <https://www.pointers-box.cc.cd> 的源代码。网站负责发布平台公告、版本更新日志、客户端下载入口与使用说明。

## 站点内容

- **首页 / 动态**：平台公告与日常动态
- **博客**：版本发布文章与版本更新日志（置顶）
- **下载**：Windows 安装版、便携版与 Android 版下载入口（GitHub / Gitee / 蓝奏云）
- **项目**：Pointers-BOX 客户端项目介绍
- **关于**：平台介绍、使用说明与社区入口

## 技术栈

- Astro 静态站点，构建产物为纯静态文件
- Svelte 5 交互组件 + Tailwind CSS
- 站内搜索由 Pagefind 在构建期生成索引

## 本地运行

环境要求：Node.js ≥ 22、pnpm 11

```bash
pnpm install
pnpm dev      # 开发预览，默认 http://localhost:4321
pnpm build    # 构建到 dist/
pnpm preview  # 预览构建产物
```

## 内容维护

- **文章**：`src/content/posts/*.md`，`pinned: true` 置顶；也可用 `pnpm new-post` 创建
- **动态**：`src/content/dynamic/*.md`；也可用 `pnpm new-dynamic` 创建
- **项目**：`src/content/projects/*.md`
- **站点配置**：`src/config/` 下按页面拆分——站点信息 `siteConfig.ts`、导航 `navBarConfig.ts`、侧边栏 `sidebarConfig.ts`、公告 `announcementConfig.ts`、壁纸 `backgroundWallpaper.ts`、音乐 `musicConfig.ts`
- **图片与静态资源**：`public/`

## 部署

`pnpm build` 生成 `dist/` 纯静态目录，推送到仓库后由托管平台自动构建部署。

## 相关链接

- 官网：<https://www.pointers-box.cc.cd>
- 客户端仓库：<https://github.com/PointersMZX/Pointers-BOX>
- Gitee 镜像：<https://gitee.com/PointersMZX/Pointers-BOX>
- 社区 QQ 群：<https://qm.qq.com/q/DGf5XI9jgW>

## 版权

© 2026 Pointers-BOX. All Rights Reserved.
