# GitHub Mobile で失敗した Actions チェックを Copilot クラウドエージェントで修正可能に

## 日付

2026-07-23

## ステータス

GA

## 概要

GitHub Mobile から PR の失敗した GitHub Actions チェックに対して、Copilot クラウドエージェントによる調査・修正を直接実行可能に。モバイルからの CI/CD 問題解決ワークフローが大幅に効率化。

## 詳細

### 主な機能

- **「Fix with Copilot」ボタン**: 失敗したチェックの通知画面に新しいボタンが追加され、ワンタップでエージェントによる修正を開始
- **自動分析と修正**: Copilot クラウドエージェントがログと PR の状態を分析し、修正内容を含む新しい PR をスタックして作成
- **レビューとマージ**: 提案された修正の差分を確認し、チェックを再実行してからマージが可能
- **iOS / Android 対応**: 最新の GitHub Mobile アプリ（iOS・Android）で利用可能

### ワークフロー

1. PR の Actions チェックが失敗する
2. GitHub Mobile で失敗通知を受け取る
3. 「Fix with Copilot」をタップ
4. Copilot クラウドエージェントがログを分析し修正を試行
5. 既存 PR の上にスタックされた修正 PR が作成される
6. 差分をレビューしてマージ

### 影響

- デスクトップ環境に戻ることなく、外出先からビルド失敗を迅速に解決可能
- コンテキストスイッチを削減し、マージサイクルの高速化に寄与

## 参考リンク

- [GitHub Mobile: Fix failing Actions checks with Copilot cloud agent](https://github.blog/changelog/2026-07-23-github-mobile-fix-failing-actions-checks-with-copilot-cloud-agent/)
