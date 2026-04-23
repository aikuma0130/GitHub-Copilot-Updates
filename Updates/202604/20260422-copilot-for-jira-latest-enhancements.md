# GitHub Copilot for Jira の最新エンハンスメント

## 日付

2026-04-22

## ステータス

Public Preview

## 概要

GitHub Copilot cloud agent の Jira 連携がさらに強化され、カスタムエージェント、カスタムフィールド、ブランチ命名規則、スペースレベルの指示、Jira 上でのレビュー通知に対応しました。

## 詳細

### カスタムエージェント

Jira チケットからリポジトリのカスタムエージェントを指定してタスクを実行できるようになりました。チーム固有のニーズに合わせて Copilot cloud agent の動作をカスタマイズできます。

### カスタムフィールド

Copilot cloud agent が Atlassian のカスタムフィールド（受け入れ条件など）の内容を読み取り、コンテキストとして活用できるようになりました。より構造化された情報をエージェントに提供できます。

### カスタムブランチ命名規則

Atlassian チケットで指定されたブランチ命名規則を Copilot cloud agent が読み取り、PR 作成時に従うようになりました。既存のワークフローとの一貫性が保たれます。

### カスタムインストラクション

Atlassian スペースレベルで Copilot cloud agent に対する包括的な指示を定義できるようになりました。対象リポジトリ、ブランチ命名規則、優先モデル、使用エージェントなどのデフォルトを設定可能です。

### Jira でのレビューリクエスト通知

Copilot cloud agent がドラフト PR を作成しレビューをリクエストすると、Jira Issue にコメントが投稿されるようになりました。PR を開いていなくてもレビュー準備完了を把握できます。

## 参考リンク

- [GitHub Copilot for Jira: Our latest enhancements](https://github.blog/changelog/2026-04-22-github-copilot-for-jira-our-latest-enhancements/)
- [Atlassian Marketplace リスティング](https://marketplace.atlassian.com/apps/1582455624/github-copilot-for-jira)
- [Jira 連携ドキュメント](https://docs.github.com/copilot/how-tos/use-copilot-agents/cloud-agent/integrate-cloud-agent-with-jira)
