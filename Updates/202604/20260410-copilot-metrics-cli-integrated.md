# Copilot CLI アクティビティが利用メトリクスの合計と機能別内訳に統合

## 日付

2026-04-10

## ステータス

GA

## 概要

Copilot CLI のアクティビティがトップレベルの合計値と機能別の内訳に統合され、IDE と CLI を合算した統一的な Copilot 利用状況の把握が可能になりました。

## 詳細

これまでの CLI メトリクスリリースでは、`totals_by_cli` セクションが独立して追加されており、IDE 活動とは別に CLI アクティビティが報告されていました。今回のアップデートにより、CLI アクティビティが既存のメトリクスに統合されます。

### 変更内容

**トップレベル合計値に CLI が含まれるようになったフィールド:**

- `code_generation_activity_count`
- `code_acceptance_activity_count`
- `user_initiated_interaction_count`
- `loc_added_sum` / `loc_deleted_sum`

**機能別内訳での CLI の表示:**

`feature=copilot_cli` として以下に表示されます：
- `totals_by_feature`
- `totals_by_model_feature`
- `totals_by_language_feature`
- `totals_by_language_model`

CLI は `totals_by_ide` からは除外されます。既存の `totals_by_cli` セクションおよびユーザー別 CLI フィールドは変更されません。

### 重要な注意点

トップレベル合計値の意味が変更されています。IDE のみのアクティビティを前提としたダッシュボードやレポートがある場合、CLI の寄与分が加わり数値が増加します。これらの値に依存するしきい値や比較がある場合はレビューが必要です。

### 主なメリット

- **統一された Copilot 利用状況**: トップレベルの合計値が全サーフェスでの Copilot アクティビティを反映
- **CLI と他の機能の比較**: `totals_by_feature` 内で CLI アクティビティをコード補完などと並べて確認可能
- **手動集計が不要に**: 以前必要だった `totals_by_cli` と IDE 合計値の手動結合が API 側で処理されるように

## 参考リンク

- [Copilot CLI activity now included in usage metrics totals and feature breakdowns](https://github.blog/changelog/2026-04-10-copilot-cli-activity-now-included-in-usage-metrics-totals-and-feature-breakdowns)
- [Copilot usage metrics API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
