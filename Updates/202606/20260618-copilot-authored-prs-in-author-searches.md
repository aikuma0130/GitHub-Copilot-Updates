# Copilot が作成した PR が作者検索に含まれるように

## 日付

2026-06-18

## ステータス

GA

## 概要

`author:` フィルターによる PR 検索で、Copilot クラウドエージェントがユーザーの代わりに作成したプルリクエストも結果に含まれるようになった。

## 詳細

### 変更内容

- `author:[username]` または `author:@me` を使用した PR 検索で、人間が作成した PR と Copilot が作成した PR が一緒に返されるようになった
- `Created by me` ビューなどのデフォルト PR クエリにも、Copilot が作成した PR が自動的に含まれる
- 複数の検索や複雑なクエリを使わずに、ユーザーが担当する全 PR を一度に確認可能

### 対応プラットフォーム

- github.com UI（現在利用可能）
- GitHub Mobile（現在利用可能）
- REST API / GraphQL API（2026年7月16日にロールアウト予定）

### 関連する変更

[グローバル PR ダッシュボード](https://github.blog/changelog/2026-04-23-global-pull-requests-dashboard-moves-to-opt-out-public-preview/)では、Copilot PR の著者が「username with Copilot」として帰属表示される。

## 参考リンク

- [Copilot-authored pull requests now included in author searches](https://github.blog/changelog/2026-06-18-copilot-authored-pull-requests-now-included-in-author-searches/)
