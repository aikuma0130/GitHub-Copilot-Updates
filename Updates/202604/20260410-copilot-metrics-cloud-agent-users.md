# Copilot 利用メトリクスに cloud agent アクティブユーザー数の集計を追加

## 日付

2026-04-10

## ステータス

GA

## 概要

Copilot 利用メトリクス API の Enterprise・Organization レポートに、Copilot cloud agent のアクティブユーザー数を集計する3つの新フィールドが追加されました。

## 詳細

[cloud agent アクティブユーザー識別](https://github.blog/changelog/2026-03-25-copilot-usage-metrics-now-identify-active-copilot-coding-agent-users/)の発表に続き、1日および28日レポートに以下のフィールドが追加されました。

### 新フィールド

| フィールド | 説明 |
|-----------|------|
| `daily_active_copilot_cloud_agent_users` | その日に Copilot cloud agent を使用したユニークユーザー数 |
| `weekly_active_copilot_cloud_agent_users` | 過去7日間に Copilot cloud agent を使用したユニークユーザー数 |
| `monthly_active_copilot_cloud_agent_users` | 過去28日間に Copilot cloud agent を使用したユニークユーザー数 |

これらのフィールドは nullable で、データが利用可能な場合はカウント（ゼロを含む）を返し、データが存在しない場合は `null` を返します。

### 主なメリット

- **導入状況の一目把握**: ユーザーレベルのデータを自分で集計することなく、cloud agent のアクティブユーザー数を確認可能
- **時間枠での比較**: 日次・週次・月次のカウントで導入トレンドの把握やロールアウト効果の測定が可能
- **全体像の把握**: 既存の `monthly_active_agent_users`（IDE エージェントモード）やユーザーレベルの `used_copilot_coding_agent` フラグと併せて、Copilot 導入の全体像を確認可能

## 参考リンク

- [Copilot usage metrics now aggregate Copilot cloud agent active user counts](https://github.blog/changelog/2026-04-10-copilot-usage-metrics-now-aggregate-copilot-cloud-agent-active-user-counts)
- [Copilot usage metrics API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
