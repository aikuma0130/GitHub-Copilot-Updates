# ワンクリックで GitHub Actions の失敗を Copilot Cloud Agent が修正

## 日付

2026-05-18

## ステータス

GA

## 概要

GitHub Actions ジョブが失敗した際、Copilot Business / Enterprise ユーザーは「Fix with Copilot」ボタンをワンクリックするだけで Copilot Cloud Agent に修正を依頼できるようになった。

## 詳細

### 変更内容

ワークフロー実行ログページに「Fix with Copilot」ボタンが追加された。クリックすると Copilot Cloud Agent が以下を自動実行する：

1. 失敗原因の調査
2. ブランチへの修正プッシュ
3. 完了時にユーザーへのレビュー依頼タグ付け

すべてクラウドベースの開発環境で処理されるため、開発者はコンテキストスイッチなしに本来の作業に集中できる。

### ユースケース

- テストの修正
- リンターエラーの修正
- ビルド失敗の解消

### 前提条件

- Copilot Business または Copilot Enterprise サブスクリプション
- 組織の管理者が Copilot Cloud Agent を有効にしていること

## 参考リンク

- [One-click fixes for failing Actions with Copilot cloud agent](https://github.blog/changelog/2026-05-18-one-click-fixes-for-failing-actions-with-copilot-cloud-agent/)
- [Enabling Copilot cloud agent](https://docs.github.com/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/enable-copilot-cloud-agent)
- [Starting GitHub Copilot sessions](https://docs.github.com/copilot/how-tos/use-copilot-agents/cloud-agent/start-copilot-sessions#asking-copilot-to-fix-a-failing-github-actions-workflow-run)
