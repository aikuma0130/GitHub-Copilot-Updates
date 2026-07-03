# Copilot エージェントセッションストリーミングがパブリックプレビューに

## 日付

2026-07-02

## ステータス

Public Preview

## 概要

GitHub Enterprise Cloud のマネージドユーザー向けに、全 Copilot クライアントのエージェントセッションデータ（プロンプト、レスポンス、ツール呼び出し）をストリーミングまたは REST API 経由で取得可能に。

## 詳細

Enterprise マネージドユーザーを持つ GitHub Enterprise Cloud のお客様が、以下を含む全 Copilot クライアントのエージェントセッションデータにアクセスできるようになった。

### 対象クライアント

- github.com および ghe.com 上のクラウドエージェント
- GitHub Copilot CLI
- Visual Studio Code
- Visual Studio
- JetBrains、Eclipse などのパートナー IDE

### データアクセス方法

#### ストリーミングエンドポイント

- 監査ログ設定からイベントコレクターまたは SIEM ツールへのストリーミング接続を設定
- Microsoft Purview もストリーミングエンドポイントとしてパブリックプレビューで利用可能

#### REST API

- エンドポイント: `GET /enterprises/{enterprise}/copilot/usage-records`
- 過去48時間分のセッションデータをオンデマンドで取得可能

### 有効化手順

AI Controls の Copilot サブページで以下を「Enable everywhere」に設定:
- Copilot Usage Records Streaming
- Copilot Usage Records API

## 参考リンク

- [Copilot agent session streaming is now in public preview](https://github.blog/changelog/2026-07-02-copilot-agent-session-streaming-is-now-in-public-preview/)
- [Audit log streaming documentation](https://docs.github.com/enterprise-cloud@latest/admin/monitoring-activity-in-your-enterprise/reviewing-audit-logs-for-your-enterprise/streaming-the-audit-log-for-your-enterprise)
- [Copilot Usage Records REST API](https://docs.github.com/en/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics)
