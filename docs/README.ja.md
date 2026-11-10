# Pointers-BOX 公式サイト

このリポジトリは Pointers-BOX 公式サイト <https://www.pointers-box.cc.cd> のソースコードです。プラットフォームのお知らせ、バージョン更新履歴、クライアントのダウンロード入口、利用ガイドを掲載しています。

## サイト構成

- **ホーム / 動向**：プラットフォームのお知らせと日々の動向
- **ブログ**：リリース記事とバージョン更新履歴（ピン留め）
- **ダウンロード**：Windows インストーラー、ポータブル版、Android 版のダウンロード入口（GitHub / Gitee / 藍奏雲）
- **プロジェクト**：Pointers-BOX クライアントの紹介
- **概要**：プラットフォーム紹介、利用ガイド、コミュニティ入口

## 技術スタック

- Astro による静的サイト。ビルド成果物は純粋な静的ファイル
- Svelte 5 のインタラクティブコンポーネント + Tailwind CSS
- サイト内検索は Pagefind がビルド時にインデックスを生成

## ローカル実行

必要環境：Node.js ≥ 22、pnpm 11

```bash
pnpm install
pnpm dev      # 開発プレビュー（既定 http://localhost:4321）
pnpm build    # dist/ にビルド
pnpm preview  # ビルド成果物をプレビュー
```

## コンテンツ管理

- **記事**：`src/content/posts/*.md`、`pinned: true` でピン留め、`pnpm new-post` でも作成可
- **動向**：`src/content/dynamic/*.md`、`pnpm new-dynamic` でも作成可
- **プロジェクト**：`src/content/projects/*.md`
- **サイト設定**：`src/config/` にページ別に分割——サイト情報 `siteConfig.ts`、ナビ `navBarConfig.ts`、サイドバー `sidebarConfig.ts`、お知らせ `announcementConfig.ts`、壁紙 `backgroundWallpaper.ts`、音楽 `musicConfig.ts`
- **画像・静的アセット**：`public/`

## デプロイ

`pnpm build` で `dist/` を生成します。リポジトリへプッシュすると、ホスティング側が自動でビルド・デプロイします。

## リンク

- 公式サイト：<https://www.pointers-box.cc.cd>
- クライアントリポジトリ：<https://github.com/PointersMZX/Pointers-BOX>
- Gitee ミラー（リリース版のダウンロード）：<https://gitee.com/PointersMZX/Pointers-BOX>
- コミュニティ QQ グループ：<https://qm.qq.com/q/DGf5XI9jgW>

## 著作権

© 2026 Pointers-BOX. All Rights Reserved.
