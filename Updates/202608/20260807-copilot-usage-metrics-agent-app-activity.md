# Copilot 使用状況メトリクス API にエージェントアプリのアクティビティ追加

## 日付

2026-08-07

## ステータス

GA

## 概要

Copilot 使用状況メトリクス API がサードパーティエージェントアプリのアクティビティを個別に報告するようになり、エージェントごとの利用状況を追跡可能に。

## 詳細

### 新しいフィールド

`totals_by_3rd_party_agent` 配列が追加され、各エージェントアプリごとに以下の情報が含まれます：

- **`agent_name`**: エージェントの表示名（変更される可能性あり）
- **`agent_id`**: 安定した識別子。レポート期間をまたいだ結合にはこのフィールドを使用
- **`user_initiated_interaction_count`**: ユーザーが開始したエージェントアプリジョブの数
- **`session_count`**: エージェントアプリセッション数（組織/エンタープライズ集約レポートのみ）

### 対応レポート

- エンタープライズ、組織、エンタープライズユーザー、組織ユーザーの 1 日および 28 日レポート

### 重要な注意事項

- ネストされた `user_initiated_interaction_count` はトップレベルの同名フィールドとは異なるもの。合算不可
- エージェントアプリのアクティビティがない場合、`totals_by_3rd_party_agent` フィールドは省略される
- 既存フィールドへの影響なし（後方互換性あり）

## 参考リンク

- [Copilot usage metrics API adds agent app activity](https://github.blog/changelog/2026-08-07-copilot-usage-metrics-api-adds-agent-app-activity/)
- [Copilot usage metrics API documentation](https://docs.github.com/rest/copilot/copilot-usage-metrics)
