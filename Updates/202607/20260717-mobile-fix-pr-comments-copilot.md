# GitHub Mobile で PR コメントを Copilot クラウドエージェントで修正可能に

## 日付

2026-07-17

## ステータス

GA

## 概要

GitHub Mobile でプルリクエストのコードレビューコメントから直接「Fix with Copilot」を実行可能に。モバイルからコードレビュー指摘の修正をクラウドエージェントに委任できる。

## 詳細

### 機能概要

GitHub Mobile（iOS / Android）のプルリクエスト画面で、Copilot Code Review のコメントから直接「Fix with Copilot」ボタンをタップ可能に。メインビューおよびコメント詳細画面の両方からアクセスできる。

### 動作フロー

1. プルリクエストの Code Review コメントを表示
2. 「Fix with Copilot」ボタンをタップ
3. Copilot クラウドエージェントへの修正リクエストが自動作成・送信
4. エージェントがコメントの内容に基づいてコード修正を実行

### ユースケース

- コードレビュー指摘の迅速な修正
- GitHub Actions の失敗修正
- テストの追加
- フォローアップのコード変更
- @copilot メンションによるカスタム指示の送信

### メリット

- PC を離れている場面でも PR のブロック解除が可能
- レビューから修正までのフィードバックループを短縮
- 開発ワークフローの中断を最小化

## 参考リンク

- [GitHub Mobile: Fix pull request comments with Copilot cloud agent](https://github.blog/changelog/2026-07-17-github-mobile-fix-pull-request-comments-with-copilot-cloud-agent/)
