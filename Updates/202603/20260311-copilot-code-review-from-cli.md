# GitHub CLI から Copilot Code Review をリクエスト可能に

## 日付

2026-03-11

## ステータス

Improvement

## 概要

GitHub CLI v2.88.0 以降で `gh pr edit --add-reviewer @copilot` により、ターミナルから直接 Copilot にコードレビューをリクエスト可能に。

## 詳細

GitHub CLI から直接 Copilot にコードレビューをリクエストできるようになりました。`gh pr edit --add-reviewer @copilot` でノンインタラクティブに、またはインタラクティブプロンプトで Copilot をレビュアーとして選択できます。`gh pr create` でも利用可能。GitHub CLI v2.88.0 以降が必要です。

また、レビュアーやアサイニーの選択体験も改善され、入力に応じた検索ベースの体験に変更されました。

## 参考リンク

- [Request Copilot code review from GitHub CLI](https://github.blog/changelog/2026-03-11-request-copilot-code-review-from-github-cli)
