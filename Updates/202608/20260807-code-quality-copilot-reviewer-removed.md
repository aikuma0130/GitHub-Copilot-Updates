# GitHub Code Quality が Copilot をレビュアーとして自動追加しなくなった

## 日付

2026-08-07

## ステータス

変更

## 概要

GitHub Code Quality を有効にしても Copilot コードレビューが自動でリクエストされなくなった。既存のルールセットも無効化済み。

## 詳細

### 背景

2026年7月20日の Code Quality GA 時に、有効化すると `Code Quality Copilot review for default branch` ルールセットが作成され、Copilot が自動レビュアーとして追加されていました。ユーザーからのフィードバックを受け、この動作が撤回されました。

### 無効化された設定

- **Automatically request Copilot code review**: すべての PR で Copilot レビューを自動リクエスト
- **Review new pushes**: PR への新しいプッシュごとに再レビューをリクエスト
- **Review draft pull requests**: ドラフト PR でもレビューをリクエスト

### 注意事項

- ユーザーが編集済みのルールセットは変更されない
- ルールセットは残るが設定は無効化。削除は手動で可能
- Copilot コードレビュー自体は引き続き利用可能。手動でルールセットを再設定すれば自動レビューを復活可能

### 対象

- GitHub Enterprise Cloud および GitHub Team

## 参考リンク

- [GitHub Code Quality no longer adds Copilot as a reviewer](https://github.blog/changelog/2026-08-07-github-code-quality-no-longer-adds-copilot-as-a-reviewer/)
- [Configuring automatic code review by Copilot](https://docs.github.com/copilot/how-tos/copilot-on-github/set-up-copilot/configure-automatic-review#configuring-automatic-code-review-for-a-single-repository)
