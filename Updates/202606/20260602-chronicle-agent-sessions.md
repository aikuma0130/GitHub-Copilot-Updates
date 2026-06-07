# /chronicle でエージェントセッションのインサイトを取得

## 日付

2026-06-02

## ステータス

GA

## 概要

/chronicle コマンドで Copilot セッション履歴を横断的にクエリし、スタンドアップサマリーやパーソナライズドティップス、カスタムインストラクションを生成可能に。セッション同期で GitHub アカウントに紐づけ。

## 詳細

### /chronicle とは

Copilot で行った作業（バグ修正、コードレビュー、機能開発等）の履歴を活用し、以下の機能を提供する。

### 利用可能なコマンド

- `/chronicle standup`: 最近のセッションを要約したレポートを生成
- `/chronicle tips`: パーソナライズされた Copilot 活用のヒントを提供
- `/chronicle improve`: セッション履歴を分析し、Copilot の理解を向上させるカスタムインストラクションを生成
- `/chronicle search`: 過去のセッションをクエリで検索

### 対応プラットフォーム

- GitHub Copilot アプリ
- github.com
- VS Code
- JetBrains

### セッション同期

- ローカルセッションが GitHub アカウントに同期され、リポジトリの Agents タブで表示可能
- セッションはデフォルトで非公開
- `/share gist` や github.com の Sharing settings で閲覧専用共有が可能
- Business / Enterprise ユーザーは管理者がローカルセッション同期を有効化する必要あり

## 参考リンク

- [Gain insights across your agent sessions with /chronicle](https://github.blog/changelog/2026-06-02-gain-insights-across-your-agent-sessions-with-chronicle/)
- [/chronicle ドキュメント](https://docs.github.com/copilot/concepts/agents/copilot-cli/chronicle)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/197305)
