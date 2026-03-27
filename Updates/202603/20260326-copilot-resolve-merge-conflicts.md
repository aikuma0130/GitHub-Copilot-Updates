# @copilot でプルリクエストのマージコンフリクトを解決

## 日付

2026-03-26

## ステータス

GA

## 概要

Copilot coding agent がプルリクエストのマージコンフリクトを解決できるようになりました。`@copilot Merge in main and resolve the conflicts` のようにコメントで指示するだけで対応できます。

## 詳細

Copilot coding agent がプルリクエストのマージコンフリクトを解決できるようになりました。

PR コメントで `@copilot Merge in main and resolve the conflicts` と指示するだけで、エージェントがクラウドベースの開発環境で変更を行い、ビルドとテストの通過を確認してからプッシュします。

その他にも以下の操作が可能です：
- **失敗した GitHub Actions ワークフローの修正**: `@copilot Fix the failing tests`
- **コードレビューコメントへの対応**: `@copilot Address this comment`
- **その他の変更**: `@copilot Add a unit test covering the case when the model argument is missing`

すべての有料 Copilot プランで利用可能です。

## 参考リンク

- [Ask @copilot to resolve merge conflicts on pull requests](https://github.blog/changelog/2026-03-26-ask-copilot-to-resolve-merge-conflicts-on-pull-requests)
