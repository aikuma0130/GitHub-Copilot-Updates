# Copilot Coding Agent の検証ツールを設定可能に

## 日付

2026-03-18

## ステータス

Improvement

## 概要

Copilot Coding Agent が使用する検証ツール（CodeQL、Secret Scanning、Code Review 等）をリポジトリ設定から無効化可能に。

## 詳細

Copilot Coding Agent はコード作成時に自動でテスト、リンター、GitHub のセキュリティ検証ツール（CodeQL、GitHub Advisory Database、Secret Scanning、Copilot Code Review）を実行します。これらは無料でデフォルト有効ですが、特定のチェックを無効化したい場合（例: CodeQL 分析に時間がかかるプロジェクト）のために、リポジトリ管理者がリポジトリ設定の **Copilot → Coding agent** セクションから検証ツールを構成できるようになりました。

## 参考リンク

- [Configure Copilot coding agent's validation tools](https://github.blog/changelog/2026-03-18-configure-copilot-coding-agents-validation-tools)
