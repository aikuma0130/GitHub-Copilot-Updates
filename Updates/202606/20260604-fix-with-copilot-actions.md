# Fix with Copilot が Pro、Pro+、Max プランで利用可能に

## 日付

2026-06-04

## ステータス

GA

## 概要

GitHub Actions ジョブの失敗時にワンクリックで Copilot クラウドエージェントが修正を調査・プッシュ。テストやリンターの修正作業を自動化できる。

## 詳細

GitHub Actions ジョブが失敗した際、Copilot Pro、Pro+、Max サブスクライバーはワンクリックで Copilot クラウドエージェントに修正を依頼できるようになった。

### ワークフロー

1. ワークフロー実行ログページの「**Fix with Copilot**」ボタンをクリック
2. Copilot が失敗の原因を調査
3. クラウドベースの開発環境から修正をブランチにプッシュ
4. 完了後、レビューのためにユーザーをタグ付け

### 対象シナリオ

- テストの修正
- リンターエラーの修正
- 依存関係バージョンの不一致修正
- その他の軽微なコード変更

この機能により、開発者はシンプルだが時間のかかる修正作業を Copilot に委託し、本来の開発作業に集中できる。

## 参考リンク

- [Fix with Copilot for failing Actions now in Pro, Pro+, and Max](https://github.blog/changelog/2026-06-04-fix-with-copilot-for-failing-actions-now-in-pro-pro-and-max/)
- [Starting GitHub Copilot sessions](https://docs.github.com/copilot/how-tos/use-copilot-agents/cloud-agent/start-copilot-sessions)
