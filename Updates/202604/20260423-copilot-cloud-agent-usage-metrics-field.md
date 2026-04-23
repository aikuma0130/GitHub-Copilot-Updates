# Copilot 利用メトリクス API に cloud agent フィールドを追加

## 日付

2026-04-23

## ステータス

GA

## 概要

Copilot coding agent から Copilot cloud agent へのリブランドに伴い、利用メトリクス API にユーザーレベルの `used_copilot_cloud_agent` フィールドが追加されました。

## 詳細

### 新フィールド

| フィールド | 説明 |
|-----------|------|
| `used_copilot_cloud_agent` | レポート期間中にユーザーが Copilot cloud agent を利用したかどうか（boolean、nullable） |

### 利用可能なレポート

- Enterprise ユーザーレポート（1日・28日ローリングウィンドウ）
- Organization ユーザーレポート（1日・28日ローリングウィンドウ）

### 後方互換性

- 既存の `used_copilot_coding_agent` フィールドは引き続き利用可能
- 両フィールドは同じ値を返し、共存します
- `used_copilot_coding_agent` は 2026年8月1日まで非推奨になりません

### 移行について

- ダッシュボードやインテグレーションを新フィールド名に移行可能
- 移行は任意のタイミングで実施可能

## 参考リンク

- [Copilot cloud agent fields added to usage metrics](https://github.blog/changelog/2026-04-23-copilot-cloud-agent-fields-added-to-usage-metrics/)
- [Copilot usage metrics API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
