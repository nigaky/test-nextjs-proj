# タスクリスト

## 1. 環境構築

- [ ] Next.jsプロジェクトの初期化 (`npx create-next-app mypj --ts --eslint --no-tailwind --no-src-dir --app --no-import-alias --turbopack`) 
- [ ] 必要なライブラリのインストール (`microcms-js-sdk`, `date-fns` など)
- [ ] リンターとフォーマッターの設定 (ESLint, Prettier)

## 2. 基本構造の実装

- [ ] 設計に基づいたディレクトリ構造の作成 (`components`, `libs/types`)
- [ ] microCMSクライアントの作成 (`libs/client.ts`)
- [ ] 型定義ファイルの作成 (`libs/types/news.ts`, `libs/types/member.ts`)
- [ ] グローバルCSSの初期設定 (`app/globals.css`)

## 3. 共通コンポーネントの実装

- [ ] `Header` コンポーネントの作成 (`components/Header.tsx`)
- [ ] `Footer` コンポーネントの作成 (`components/Footer.tsx`)
- [ ] `Layout` コンポーネントの作成 (`components/Layout.tsx`)
- [ ] `app/layout.tsx` で `Layout` コンポーネントを使用するように設定

## 4. ページ実装

- [ ] **トップページ** (`app/page.tsx`)
    - [ ] `microCMS` の `news` APIからお知らせの最新数件を取得
    - [ ] お知らせ一覧を画面に表示
- [ ] **メンバーページ** (`app/members/page.tsx`)
    - [ ] `app/members` ディレクトリの作成
    - [ ] `microCMS` の `members` APIから全てのメンバーを取得
    - [ ] メンバー一覧を画面に表示
- [ ] **ニュース一覧ページ** (`app/news/page.tsx`)
    - [ ] `app/news` ディレクトリの作成
    - [ ] `microCMS` の `news` APIから全てのニュースを取得
    - [ ] ニュースをリスト形式で表示
    - [ ] ページネーションの実装
- [ ] **ニュース詳細ページ** (`app/news/[id]/page.tsx`)
    - [ ] `app/news/[id]` ディレクトリの作成
    - [ ] `generateStaticParams` で動的ルートを生成
    - [ ] 指定されたIDのニュースデータを `microCMS` の `news` APIから取得
    - [ ] ニュースの内容を表示

## 5. 仕上げ

- [ ] 全ページのレスポンシブ対応
- [ ] 全体的な動作確認とデバッグ