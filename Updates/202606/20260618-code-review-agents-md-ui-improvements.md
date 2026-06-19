# Copilot Code Review: AGENTS.md サポートと UI 改善

## 日付

2026-06-18

## ステータス

GA

## 概要

Copilot Code Review がリポジトリルートの `AGENTS.md` ファイルを自動的に参照してレビューフィードバックを生成するようになり、ドラフト PR でのレビューリクエストやタイムラインの UI も改善された。

## 詳細

### AGENTS.md サポート

リポジトリルートに `AGENTS.md` ファイルを配置すると、Copilot Code Review がそのコンテキストを自動的にワークフローの一部として活用する。これにより、リポジトリの規約や期待に沿ったレビューフィードバックを得やすくなる。

- リポジトリルートの `AGENTS.md` を読み取り
- ファイル内の関連する指示をレビューフィードバック生成時に使用

### UI の改善

#### ドラフト PR でのレビューリクエストが容易に

ドラフトプルリクエストで Copilot Code Review をリクエストする際、レビュアーピッカーに **Request** ボタンが直接表示されるようになった。Copilot を検索する手間なく、ワンクリックでレビューをリクエスト可能。

#### タイムラインイベントの折りたたみ

プルリクエストの Conversation タブで、Copilot Code Review のタイムラインイベントが折りたたまれて表示されるようになり、会話タブのノイズが軽減された。

## 参考リンク

- [Copilot code review: AGENTS.md support and UI improvements](https://github.blog/changelog/2026-06-18-copilot-code-review-agents-md-support-and-ui-improvements/)
