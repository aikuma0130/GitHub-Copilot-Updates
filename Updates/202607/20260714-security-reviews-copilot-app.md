# GitHub Copilot アプリでセキュリティレビューが利用可能に

## 日付

2026-07-14

## ステータス

Public Preview

## 概要

GitHub Copilot アプリで `/security-review` スラッシュコマンドがパブリックプレビューとして提供開始。作業中のコード変更に対して、Copilot アプリから直接セキュリティレビューを実行できるようになった。

## 詳細

### 機能概要

`/security-review` コマンドは、現在の作業ストリームの変更を分析し以下を返す:

- 重大度と信頼度でスコアリングされた高信頼度のセキュリティ所見
- Copilot を離れることなく適用・再検証可能なアクション可能な提案
- 重要な問題を優先的に修正できるフォーカスされたビュー

### 検出対象

一般的で影響の大きい脆弱性クラスを検出するようチューニングされている:

- インジェクション攻撃
- クロスサイトスクリプティング (XSS)
- 安全でないデータ処理
- パストラバーサル
- 弱い暗号化

### 位置づけ

GitHub Code Scanning、Dependabot、Secret Scanning を補完し、ローカル変更に対する軽量なオンデマンドチェックを提供する。コードがランディングする前に問題をキャッチするための手段。

### 利用方法

Copilot アプリでプロジェクトを開き、コード変更を行い、`/security-review` を実行。パブリックプレビュー期間中は Copilot Free、Pro、Business、Enterprise の全ユーザーが利用可能。

## 参考リンク

- [Security reviews now available in the GitHub Copilot app](https://github.blog/changelog/2026-07-14-security-reviews-now-available-in-the-github-copilot-app/)
