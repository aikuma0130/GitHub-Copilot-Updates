# Copilot cloud agent でマージコンフリクトを3クリックで解決

## 日付

2026-04-13

## ステータス

GA

## 概要

GitHub.com のプルリクエスト上に新しい「Fix with Copilot」ボタンが追加され、Copilot cloud agent を使ってマージコンフリクトを3クリックで解決できるようになりました。

## 詳細

Copilot cloud agent を活用した新機能により、GitHub.com 上でマージコンフリクトの解決がこれまで以上に簡単になりました。

### 使い方

1. プルリクエストのマージボックスに表示される「**Fix with Copilot**」ボタンをクリック
2. コメントボックスにコンフリクト解決を依頼するコメントが自動入力される
3. コメントを送信すると、Copilot がコンフリクトを修正し、ビルドとテストの成功を確認した上でプッシュ

すべての処理は Copilot cloud agent 独自のクラウドベース開発環境で実行されます。

### その他の @copilot メンション機能

プルリクエストで `@copilot` をメンションすることで、以下の操作も可能です：

- **失敗した GitHub Actions ワークフローの修正**: `@copilot Fix the failing tests`
- **コードレビューコメントへの対応**: `@copilot Address this comment`
- **その他の変更**: `@copilot Add a unit test covering the case when the model argument is missing`

### 利用条件

Copilot cloud agent は全有料 Copilot プランで利用可能です。Copilot Business または Copilot Enterprise ユーザーの場合、管理者が事前に Copilot cloud agent を有効化する必要があります。

## 参考リンク

- [Fix merge conflicts in three clicks with Copilot cloud agent](https://github.blog/changelog/2026-04-13-fix-merge-conflicts-in-three-clicks-with-copilot-cloud-agent/)
- [Asking GitHub Copilot to make changes to an existing pull request](https://docs.github.com/copilot/how-tos/use-copilot-agents/cloud-agent/make-changes-to-an-existing-pr)
- [Copilot cloud agent の管理](https://docs.github.com/en/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/manage-copilot-cloud-agent)
