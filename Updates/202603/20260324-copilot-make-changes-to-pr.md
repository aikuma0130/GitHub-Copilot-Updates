# @copilot で PR に変更を依頼可能に

## 日付

2026-03-24

## ステータス

Improvement

## 概要

PR コメントで `@copilot` をメンションして変更を依頼可能に。既存 PR への直接変更プッシュに対応（以前は別 PR を作成）。

## 詳細

PR コメントで `@copilot` をメンションして変更を依頼できるようになりました。以下のようなタスクに対応：

- GitHub Actions ワークフローの失敗修正: `@copilot Fix the failing tests`
- コードレビューコメントの対応: `@copilot Address this comment`
- その他の変更: `@copilot Add a unit test covering the case when the model argument is missing`

以前は既存 PR の上に新しい PR を作成していましたが、既存 PR に直接変更をプッシュするようになりました。従来の動作が必要な場合は `@copilot open a PR to fix the failing tests` と自然言語で依頼可能。フォークからの PR は現在未対応。

## 参考リンク

- [Ask @copilot to make changes to a pull request](https://github.blog/changelog/2026-03-24-ask-copilot-to-make-changes-to-any-pull-request)
