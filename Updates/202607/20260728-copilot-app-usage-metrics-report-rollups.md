# Copilot アプリ使用メトリクスがレポートロールアップ全体に拡大

## 日付

2026-07-28

## ステータス

GA

## 概要

Copilot アプリの使用状況が使用メトリクス API のより多くのレポートロールアップに反映されるようになった。ユーザー単位の帰属表示、機能・モデル・言語別の内訳表示が追加され、全 Copilot サーフェスとの横断的な比較が可能に。

## 詳細

### 新しいメトリクス

- **`used_copilot_app`**: ユーザーが指定日に Copilot アプリでアクティブだったかどうかを示すフラグ。
- **`totals_by_copilot_app`**: ユーザー単位のセクションで `session_count`、`request_count`、`prompt_count`、および `token_usage`（`output_tokens_sum`、`prompt_tokens_sum`、`avg_tokens_per_request`）の内訳を報告。
- **`copilot_app` feature 値**: `totals_by_feature`、`totals_by_model_feature`、`totals_by_language_feature`、`totals_by_language_model` に Copilot アプリのアクティビティが表示。
- **コードアクティビティおよび行数メトリクス**: トップレベルのコード生成、コード受け入れ、追加行数、削除行数の集計に Copilot アプリのアクティビティが含まれるように。
- **`daily_active_users`**: Copilot アプリのみでアクティブだったユーザーもカウント対象に。

### 意義

以前はエンタープライズ・組織レベルの合計としてのみ表示されていた Copilot アプリの使用状況が、個別ユーザーに帰属表示され、標準的な内訳に組み込まれることで、採用者の特定やコード生成量の測定が可能に。IDE、チャット、Code Review、Coding Agent と同じフィールドでの比較も実現。

### 注意事項

- エンタープライズユーザーおよび組織ユーザーの 1 日・28 日レポートで利用可能。
- エンタープライズオーナー、課金マネージャー、組織オーナー、および Copilot メトリクス閲覧権限を持つカスタムロールで利用可能。
- 後方互換性あり。Copilot アプリのアクティビティがないユーザー・エンティティでは該当セクションが省略される。

## 参考リンク

- [GitHub Copilot app usage metrics now expand across report rollups](https://github.blog/changelog/2026-07-28-github-copilot-app-usage-metrics-now-expand-across-report-rollups/)
- [Copilot 使用メトリクス API ドキュメント](https://docs.github.com/rest/copilot/copilot-usage-metrics)
