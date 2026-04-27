# Copilot コードレビューが 2026年6月1日から GitHub Actions 分数を消費

## 日付

2026-04-27

## ステータス

Release

## 概要

2026年6月1日より、Copilot コードレビューが GitHub Actions 分数を消費するようになります。プライベートリポジトリでのレビューごとに Actions 分数が使用され、既存のプラン枠を超過した場合は標準料金で課金されます。

## 詳細

### 変更内容

2026年6月1日から、Copilot コードレビューの課金方法が以下の2つになります：

1. **AI クレジット**: 使用量ベースの課金モデルに基づく Copilot 利用分
2. **GitHub Actions 分数**: プライベートリポジトリでのレビュー実行にプラン枠の Actions 分数が消費される（パブリックリポジトリは引き続き無料）

### 対象プラン

- GitHub Copilot Pro
- GitHub Copilot Pro+
- GitHub Copilot Business
- GitHub Copilot Enterprise

ライセンスを持たないユーザーが [Organization の直接課金](https://docs.github.com/copilot/concepts/agents/code-review#enabling-code-review-for-users-without-a-license)でコードレビューを利用する場合も対象です。

### 推奨される準備

1. 現在の GitHub Actions 使用量を確認する
2. [予算・支出制限](https://docs.github.com/billing/how-tos/set-up-budgets)が想定使用量に合っているか確認する
3. [Copilot 利用メトリクス](https://docs.github.com/copilot/concepts/copilot-usage-metrics)と [Actions メトリクス](https://docs.github.com/enterprise-cloud@latest/organizations/collaborating-with-groups-in-organizations/viewing-github-actions-metrics-for-your-organization)で使用状況を監視する
4. 請求管理者やエンジニアリングリードに変更を共有する

### ランナー設定

- GitHub ホステッドランナーが有効であれば追加設定は不要
- [セルフホステッドランナー](https://docs.github.com/enterprise-cloud@latest/copilot/how-tos/copilot-on-github/set-up-copilot/configure-runners#upgrade-to-larger-github-hosted-github-actions-runners)や[ラージランナー](https://docs.github.com/enterprise-cloud@latest/copilot/how-tos/copilot-on-github/set-up-copilot/configure-runners#upgrade-to-larger-github-hosted-github-actions-runners)も利用可能（課金レートは異なる）

## 参考リンク

- [GitHub Copilot code review will start consuming GitHub Actions minutes on June 1, 2026](https://github.blog/changelog/2026-04-27-github-copilot-code-review-will-start-consuming-github-actions-minutes-on-june-1-2026)
- [コードレビューのモデルと価格](https://docs.github.com/copilot/reference/copilot-billing/models-and-pricing#github-actions-minutes-for-code-review)
