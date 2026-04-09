# Copilot コードレビュー済み PR のマージメトリクスが利用メトリクス API に追加

## 日付

2026-04-08

## ステータス

Release

## 概要

Copilot 利用メトリクス API に、Copilot コードレビューを受けた PR のマージ数とマージまでの中央値時間を追跡する2つの新しいメトリクスが追加されました。これにより、Copilot コードレビューが PR ライフサイクルに与える影響をエンドツーエンドで可視化できます。

## 詳細

2月に出荷された Copilot コーディングエージェントが作成した PR のスループット・サイクルタイムメトリクスに続き、Copilot 利用メトリクス API にコードレビュー活動に焦点を当てた2つの新しいメトリクスが追加されました。

### 新しいメトリクス

- **`pull_requests.total_merged_reviewed_by_copilot`**: 対象期間中に Copilot コードレビューを受け、かつマージされた PR の合計数
- **`pull_requests.median_minutes_to_merge_copilot_reviewed`**: Copilot コードレビューを受けた PR のみを対象とした、PR 作成からマージまでの中央値時間（分）

### 既存メトリクスとの違い

以前のリリースでは Copilot が PR を **作成（author）** する側のメトリクス（コーディングエージェントが作成した PR のマージ数とマージまでの時間）を提供していました。今回の新メトリクスは Copilot が PR を **レビュー（review）** する側の活動を捉え、Copilot コードレビューを受けた PR のマージ率とサイクルタイムをベースラインと比較できます。

### 利用可能な範囲

- 単日レポートおよび28日間ローリングウィンドウレポートの両方で利用可能
- エンタープライズおよび Organization レベルで提供
- Copilot 利用メトリクスにアクセス可能なエンタープライズ管理者および Organization オーナーが利用可能

### 重要な注意点

- これらのメトリクスには Copilot コードレビューを受けた PR のみが含まれます
- コーディングエージェントが作成した PR は既存の `pull_requests.total_merged_created_by_copilot` および `pull_requests.median_minutes_to_merge_copilot_authored` フィールドで別途追跡されます

## 参考リンク

- [Copilot-reviewed pull request merge metrics now in the usage metrics API](https://github.blog/changelog/2026-04-08-copilot-reviewed-pull-request-merge-metrics-now-in-the-usage-metrics-api)
- [Copilot usage metrics API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
