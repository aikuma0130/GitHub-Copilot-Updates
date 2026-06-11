# Copilot CLI に専用セキュリティレビューコマンドが追加

## 日付

2026-06-10

## ステータス

Experimental (Public Preview)

## 概要

Copilot CLI に `/security-review` スラッシュコマンドが追加され、ローカルのコード変更に対して AI 駆動のセキュリティレビューをターミナルから直接実行可能になった。

## 詳細

新しい `/security-review` コマンドは実験的機能としてパブリックプレビューで提供され、コードが本番環境に到達する前にセキュリティ脆弱性を迅速に検出する手段を提供する。

### 機能

- ローカルのコード変更を分析し、以下を返す:
  - 重大度と信頼度でスコアリングされた高信頼度のセキュリティ所見
  - ターミナルを離れずに適用できるアクション可能な提案
  - 既存ワークフロー内で完結するフォーカスされたレビュー

### 検出対象

インジェクション欠陥、クロスサイトスクリプティング、安全でないデータ処理、パストラバーサル、脆弱な暗号化など、一般的で影響の大きい脆弱性クラスを検出。

### 利用方法

1. Copilot CLI で実験モードを有効化
2. プロジェクトディレクトリで `/security-review` を実行

### 補足

GitHub Code Scanning、Dependabot、Secret Scanning とは独立した Copilot 駆動のスキャンであり、それらを補完する軽量なオンデマンドレビュー手段として位置付けられている。

## 参考リンク

- [Dedicated security review command now available in Copilot CLI](https://github.blog/changelog/2026-06-10-dedicated-security-review-command-now-available-in-copilot-cli/)
- [GitHub Community Discussion](https://github.com/orgs/community/discussions/196523)
