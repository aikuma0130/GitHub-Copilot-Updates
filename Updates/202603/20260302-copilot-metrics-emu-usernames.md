# Copilot メトリクスレポートで EMU ユーザー名が一貫して返されるように

## 日付

2026-03-02

## ステータス

Improvement

## 概要

Copilot 使用メトリクス API で Enterprise Managed Users (EMU) の `user_login` 値が一貫して返されるようになり、API 間のマッチングが容易に。

## 詳細

Copilot 使用メトリクスレポートで、Enterprise Managed Users (EMU) の `user_login` 値が一貫して返されるようになりました。以前は一部のレポートで `user_login` にサフィックスが含まれることがあり、GitHub API 間で結果をマッチングすることが困難でした。この改善により、API レスポンスの一貫性が向上し、データ分析が容易になります。

## 参考リンク

- [Copilot metrics reports now return consistent usernames for Enterprise Managed Users](https://github.blog/changelog/2026-03-02-copilot-metrics-reports-now-return-consistent-usernames-for-enterprise-managed-users)
