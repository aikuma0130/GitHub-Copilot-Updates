# Copilot Memory の削除・スコープ・CLI 制御が強化

## 日付

2026-05-26

## ステータス

Public Preview

## 概要

Copilot Memory に削除ガイダンスの改善、リポジトリレベルのオフスイッチ、CLI での `/memory` コマンドが追加され、メモリのスコープがキャプチャ時に明示されるようになった。

## 詳細

### 削除ガイダンス

Copilot に「忘れて」と依頼すると、メモリを削除するための適切な場所（設定ページ）を案内し、投票機能がある場合はメモリにダウンボートを付与するようになった。

### リポジトリレベルのオフスイッチ

リポジトリ管理者がリポジトリ設定の Copilot 機能コントロールから Copilot Memory を無効化可能に。無効化するとリポジトリレベルのファクトの保存・読み取りが停止する（既存ファクトは削除されない）。ユーザーレベルのプリファレンスには影響しない。

### `/memory` コマンド（Copilot CLI）

- `/memory on` — Copilot Memory を有効化
- `/memory off` — Copilot Memory を無効化
- `/memory show` — 現在のステータスを確認

設定はセッション間で永続化される。

### キャプチャ時のスコープ明示

`store_memory` の権限プロンプトで、エントリが「ユーザーレベルのプリファレンス」（自分のみに表示、リポジトリ横断で使用）か「リポジトリレベルのファクト」（リポジトリの全コントリビューターに表示）かが明示されるようになった。

### メモリの管理方法

- **ユーザーレベルのプリファレンス**: [Copilot Memory 設定](https://github.com/settings/copilot/memory) で確認・削除
- **リポジトリのファクト**: リポジトリ設定 > Copilot > Memory で確認・削除・無効化

## 参考リンク

- [Copilot Memory has more controls for deletion, scope, and the Copilot CLI](https://github.blog/changelog/2026-05-26-copilot-memory-has-more-controls-for-deletion-scope-and-the-copilot-cli/)
- [About GitHub Copilot Memory](https://docs.github.com/copilot/concepts/agents/copilot-memory)
- [Managing stored memories](https://docs.github.com/copilot/how-tos/use-copilot-agents/copilot-memory#viewing-and-deleting-repository-level-facts-and-user-level-preferences)
