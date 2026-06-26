# Copilot Code Review: 分析深度と効率性のアップデート

## 日付

2026-06-25

## ステータス

GA / Public Preview

## 概要

Copilot Code Review が Copilot CLI / SDK の組み込みファイル探索ツールを使用するようになり、レビューコスト効率が約20%改善。Medium 分析深度プレビューでは組織レベルのデフォルト設定と PR コメントへのティア表示が追加。

## 詳細

### CLI ベースのファイルツールの採用

Copilot Code Review がソースコード探索に `grep`、`rg`、`glob`、`view` といった Copilot CLI / SDK のツールを使用するようになった。従来のカスタムファイル探索ツールを置き換え、レビュー品質を維持しつつコストを約20%削減。

### Medium 分析深度の新機能（パブリックプレビュー）

Medium レビューエフォートレベルのプレビューに参加している場合、以下の新機能が利用可能：

- **PR オーバービューコメントへの Medium ティア表示**: どのレベルでレビューが実行されたかを即座に確認可能
- **組織レベルのデフォルトレビューレベル設定**: 組織管理者が未設定リポジトリのデフォルトレビューレベルを一括設定可能。個別リポジトリでのオーバーライドも引き続きサポート

### 既存ワークフローへの影響

ユーザー側の設定変更は不要。効率改善は自動的に適用される。

## 参考リンク

- [Copilot code review: Analysis depth and efficiency updates](https://github.blog/changelog/2026-06-25-copilot-code-review-analysis-depth-and-efficiency-updates/)
- [Shape Copilot code review around your team（Medium 分析深度プレビュー）](https://github.blog/changelog/2026-06-02-shape-copilot-code-review-around-your-team/)
