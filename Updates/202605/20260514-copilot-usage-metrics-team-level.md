# Copilot 使用量メトリクス API でチームレベルのメトリクスが利用可能に

## 日付

2026-05-14

## ステータス

GA

## 概要

Copilot 使用量メトリクス API に新しい「user-teams」レポートが追加され、Copilot ライセンスユーザーとチームのマッピングデータを取得可能に。既存のユーザー別使用量レポートと結合することで、チーム単位の Copilot 利用状況を集計・分析できる。

## 詳細

### 新しいエンドポイント

以下の2つの REST API エンドポイントが追加され、NDJSON レポートのダウンロード URL を返す：

- `GET /enterprises/{enterprise}/copilot/metrics/reports/user-teams-1-day`
- `GET /orgs/{org}/copilot/metrics/reports/user-teams-1-day`

### レポートの構成

user-teams レポートの各行は、特定の日におけるチームメンバーシップを表し、チームのエンタープライズまたはオーガニゼーション ID、チームスラッグ、ユーザー ID およびログインを含む。

### チームレベルメトリクスの作成方法

user-teams レポートをユーザー別使用量レポートと `user_id` と `day` で結合し、集計することでチームレベルのメトリクスを生成できる。ドキュメントには結合レシピやローリングウィンドウ集計のステップバイステップガイドが提供されている。

### 利用可能なメトリクス

IDE コード補完、チャット、Copilot CLI、Code Review、Cloud Agent アクティビティなど、全機能のチームレベル内訳が利用可能。言語、IDE、機能、モデル別の分析も可能。

### 利用可能なロール

エンタープライズ管理者、オーガニゼーションオーナー、課金マネージャー、および「View Enterprise Copilot Metrics」権限を持つカスタムロール。

### 注意事項

- チームレベルレポートは REST API のみで提供。ダッシュボードは未対応。
- Copilot シート数が5人未満のチームはレポートから除外される。
- 複数チームに所属するユーザーのアクティビティは各チームで重複してカウントされるため、チーム合計をオーガニゼーション全体の合計として使用することはできない。

## 参考リンク

- [Team-level Copilot usage metrics now available via API](https://github.blog/changelog/2026-05-14-team-level-copilot-usage-metrics-now-available-via-api/)
- [Team-level Copilot usage metrics - GitHub Docs](https://docs.github.com/enterprise-cloud@latest/copilot/reference/copilot-usage-metrics/team-level-metrics)
