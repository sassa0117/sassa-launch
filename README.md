# sassa-launch

さっさ式電脳せどりツール ローンチ統合リポジトリ

5つのリポジトリに散らばっていたローンチ関連素材を1箇所に統合。

## ディレクトリ構成

```
sassa-launch/
├── strategy/          戦略・設計（ローンチ計画/価格戦略/X戦略/配信スケジュール）
├── brand/             ブランド定義（さっさの独自要素）
├── content/           コンテンツ素材
│   ├── drafts/        配信下書き
│   └── note-articles/ note記事原稿
├── skills/            Claude Codeスキル
├── scripts/           自動化ツール（WP投稿/スクショ/一括公開）
└── reference/         参考資料（ぴっぷ式原文）
```

## 統合元

| ディレクトリ | 元リポジトリ |
|---|---|
| strategy/ | ai-skills, sken-step-mail |
| brand/ | claude-memory |
| content/drafts/ | sken-step-mail |
| content/note-articles/ | note-articles |
| skills/ | ai-skills, sken-step-mail |
| scripts/ | sedori-automation |
| reference/ | sken-step-mail |

## scripts の使い方

```bash
npm install
# .env を設定（.env.example 参照）
node scripts/publish.js     # 一括ワークフロー
node scripts/screenshot.js  # HTML → PNG変換
node scripts/wp-post.js     # WordPress投稿
```
