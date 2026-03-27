# Copilot Coding Agent のネットワーク構成変更が適用開始

## 日付

2026-03-02

## ステータス

Improvement

## 概要

Copilot Coding Agent のサブスクリプションベースのネットワークルーティング変更が適用。セルフホストランナー利用者は新しいホスト設定が必要。

## 詳細

2月13日に発表された Copilot Coding Agent のネットワーク構成変更が適用されました。セルフホストランナーや Azure プライベートネットワーキング付きの大規模ランナーを使用するチームに影響します。Copilot プランに応じて異なるホストに接続するサブスクリプションベースのルーティングが適用されます（Business: `api.business.githubcopilot.com`、Enterprise: `api.enterprise.githubcopilot.com`、Pro/Pro+: `api.individual.githubcopilot.com`）。

## 参考リンク

- [Network configuration changes for Copilot coding agent now in effect](https://github.blog/changelog/2026-03-02-network-configuration-changes-for-copilot-coding-agent-now-in-effect)
