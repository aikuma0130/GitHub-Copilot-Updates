# GitHub Copilot アプリのアクセスを専用ポリシーで管理

## 日付

2026-07-27

## ステータス

GA

## 概要

GitHub Copilot アプリに専用のアクセスポリシーが追加され、エンタープライズおよび組織レベルで Copilot CLI とは独立してアプリへのアクセスを制御可能に。

## 詳細

### 背景

これまで Copilot アプリへのアクセスは Copilot CLI ポリシーの有効化に依存していた。多くの顧客からクライアントごとに独立して管理したいという要望があり、今回 Copilot アプリと Copilot CLI それぞれに専用ポリシーが設けられた。

### ポリシーオプション

- **Enabled everywhere** — 開発者がアプリにアクセス可能（デフォルト）
- **Disabled everywhere** — エンタープライズ全体でアプリを無効化
- **Let organizations decide** — 各組織の管理者に判断を委任

### ガバナンスとの統合

- Copilot アプリは隔離されたワークスペースでエージェントセッションを実行し、変更は PR を通じて反映
- 既存のレビュー、チェック、監査履歴がそのまま適用される
- エンタープライズ管理設定（managed-settings）の対象クライアントとして VS Code、CLI に加えて Copilot アプリもサポート

### 設定方法

1. エンタープライズまたは組織の設定から **AI Controls** タブを開く
2. 「Copilot Clients」セクションに移動
3. **Copilot app** ポリシーを選択
4. 希望するオプションを選択

## 参考リンク

- [Manage GitHub Copilot app access with a dedicated policy](https://github.blog/changelog/2026-07-27-manage-github-copilot-app-access-with-a-dedicated-policy/)
- [GitHub Copilot アプリのドキュメント](https://docs.github.com/copilot/concepts/agents/github-copilot-app)
