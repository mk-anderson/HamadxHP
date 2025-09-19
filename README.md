# HamadxHP
HamadxHP's Source Code

# 企業サイト（WordPress + Vite + FLOCSS）

## プロジェクト概要
- WordPressテーマをViteでバンドル
- スタイリングはSCSS（FLOCSS準拠）
- 開発環境は Local by Flywheel を使用

## 要件定義 / 仕様
### ページ構成
- トップ
- 企業案内
- 拠点
- お知らせ
- お問い合わせ

### 機能要件
- お知らせ一覧 / 詳細
- 拠点一覧 / 詳細
- お問い合わせフォーム（バリデーション）

### 非機能要件
- 表示速度：LCP < 2.5s
- SEO：meta設定、構造化データ
- アクセスビリティ確保

## 命名規則（FLOCSS+BEM）
- レイヤー: `l-`, `c-`, `p-`, `u-`, `is-`, `has-`, `js-`
- BEM: `block__element--modifier`
- 例1: `c-card`, `c-card__title`, `c-card--featured`
- 例2:
```html
<section class="p-news-list is-loaded">
  <h2 class="c-card__title">タイトル</h2>
  <button class="c-button c-button--primary js-open-menu">送信</button>
</section>

## 開発環境構築
```bash
git clone ...
npm install
npm run dev
