# @copilot でプルリクエストに変更を依頼

## 日付

2026-03-24

## ステータス

GA

## 概要

プルリクエストのコメントで `@copilot` をメンションして変更を依頼できるようになりました。失敗したテストの修正、コードレビューへの対応など、既存の PR に直接変更をプッシュします。

## 詳細

プルリクエストで `@copilot` をメンションして変更を依頼できるようになりました。

依頼可能な作業：
- **失敗した GitHub Actions ワークフローの修正**: `@copilot Fix the failing tests`
- **コードレビューコメントへの対応**: `@copilot Address this comment`
- **その他の変更**: `@copilot Add a unit test covering the case when the model argument is missing`

Copilot coding agent はクラウドベースの開発環境で変更を行い、テストとリンターで検証後にプッシュします。

以前は既存 PR の上に新しい PR を開いていましたが、現在は既存の PR に直接プッシュします。フォークからの PR は現在サポートされていません。

## 参考リンク

- [Ask @copilot to make changes to a pull request](https://github.blog/changelog/2026-03-24-ask-copilot-to-make-changes-to-any-pull-request)
