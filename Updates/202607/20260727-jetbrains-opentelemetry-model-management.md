# GitHub Copilot for JetBrains に OpenTelemetry 設定とモデル管理が追加

## 日付

2026-07-27

## ステータス

GA

## 概要

JetBrains IDE 向け Copilot プラグインに OpenTelemetry エクスポート設定とモデル管理コントロールが追加。組織のオブザーバビリティ要件への対応とモデルガバナンスが強化された。

## 詳細

### OpenTelemetry エクスポート設定

- エージェントワークフロー向けの OpenTelemetry エクスポート設定が構成可能に
- `Settings > Tools > GitHub Copilot > Chat` からアクセス可能
- 組織のオブザーバビリティ要件に合わせたプラグイン動作の調整が可能

### モデル管理コントロール

- BYOK およびカスタムエンドポイント向けに `maxInputToken`、`maxOutputToken` などのデフォルトトークン制限を設定可能
- 組み込み Copilot モデルの有効化・無効化が可能
- コスト制御と堅牢なモデルガバナンスの実現を支援

### MCP とカスタムエージェント

- MCP サーバーとカスタムエージェントを Claude エージェントフローに直接接続可能
- 専門ツールやチーム固有のワークフローとの連携における柔軟性が向上

### その他の改善

- モデルおよびアクションピッカーの UI 一貫性向上
- セッションプロンプトの Markdown レンダリング改善
- MCP サーバーの診断機能向上

## 参考リンク

- [GitHub Copilot for JetBrains adds improved OpenTelemetry configuration and model management](https://github.blog/changelog/2026-07-27-github-copilot-for-jetbrains-adds-improvved-opentelemetry-configuration-and-model-management/)
