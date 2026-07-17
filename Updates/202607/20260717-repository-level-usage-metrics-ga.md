# リポジトリレベルの Copilot 使用メトリクスが GA

## 日付

2026-07-17

## ステータス

GA

## 概要

Copilot 使用メトリクス REST API がリポジトリレベルのアクティビティデータを提供開始。Copilot Coding Agent と Copilot Code Review の PR アクティビティを日次・リポジトリ単位で分析可能に。

## 詳細

### 新規 API エンドポイント

Copilot 使用メトリクス REST API に2つの新しいエンドポイントが追加され、リポジトリごとの日次プルリクエストアクティビティの内訳を取得可能になった。

### 対象メトリクス

- Copilot Coding Agent によるプルリクエストアクティビティ
- Copilot Code Review によるプルリクエストアクティビティ

### メリット

- 組織・エンタープライズ管理者がリポジトリ単位で Copilot の利用状況と影響度を詳細に追跡可能
- 既存のエンタープライズ・組織・チームレベルのメトリクスを補完し、より粒度の細かい分析が可能に
- 導入戦略の立案やコスト最適化の意思決定に活用可能

### アクセス要件

適切な権限（View Enterprise Copilot Metrics 等）が必要。ロールベースアクセス制御により、権限のあるメンバーのみがデータを閲覧可能。

## 参考リンク

- [Repository-level GitHub Copilot usage metrics generally available](https://github.blog/changelog/2026-07-17-repository-level-github-copilot-usage-metrics-generally-available/)
- [GitHub Copilot usage metrics](https://docs.github.com/en/copilot/concepts/copilot-usage-metrics/copilot-metrics)
