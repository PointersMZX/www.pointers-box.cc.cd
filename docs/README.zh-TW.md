# Pointers-BOX 官方網站

本倉庫是 Pointers-BOX 官方網站 <https://www.pointers-box.cc.cd> 的原始碼。網站負責發布平台公告、版本更新日誌、客戶端下載入口與使用說明。

## 網站內容

- **首頁 / 動態**：平台公告與日常動態
- **部落格**：版本發布文章與版本更新日誌（置頂）
- **下載**：Windows 安裝版、免安裝版與 Android 版下載入口（GitHub / Gitee / 藍奏雲）
- **專案**：Pointers-BOX 客戶端專案介紹
- **關於**：平台介紹、使用說明與社群入口

## 技術棧

- Astro 靜態網站，建置產物為純靜態檔案
- Svelte 5 互動元件 + Tailwind CSS
- 站內搜尋由 Pagefind 在建置期建立索引

## 本機執行

環境需求：Node.js ≥ 22、pnpm 11

```bash
pnpm install
pnpm dev      # 開發預覽，預設 http://localhost:4321
pnpm build    # 建置到 dist/
pnpm preview  # 預覽建置產物
```

## 內容維護

- **文章**：`src/content/posts/*.md`，`pinned: true` 置頂；也可用 `pnpm new-post` 建立
- **動態**：`src/content/dynamic/*.md`；也可用 `pnpm new-dynamic` 建立
- **專案**：`src/content/projects/*.md`
- **網站設定**：`src/config/` 下依頁面拆分——網站資訊 `siteConfig.ts`、導覽 `navBarConfig.ts`、側邊欄 `sidebarConfig.ts`、公告 `announcementConfig.ts`、桌布 `backgroundWallpaper.ts`、音樂 `musicConfig.ts`
- **圖片與靜態資源**：`public/`

## 部署

`pnpm build` 產生 `dist/` 純靜態目錄，推送到倉庫後由託管平台自動建置部署。

## 相關連結

- 官網：<https://www.pointers-box.cc.cd>
- 客戶端倉庫：<https://github.com/PointersMZX/Pointers-BOX>
- Gitee 鏡像（版本下載）：<https://gitee.com/PointersMZX/Pointers-BOX>
- 社群 QQ 群：<https://qm.qq.com/q/DGf5XI9jgW>

## 版權

© 2026 Pointers-BOX. All Rights Reserved.
