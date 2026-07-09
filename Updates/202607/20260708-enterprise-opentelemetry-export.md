# エンタープライズ管理の OpenTelemetry エクスポートが VS Code と CLI で利用可能に

## 日付

2026-07-08

## ステータス

GA

## 概要

組織が GitHub Copilot の OpenTelemetry データの送信先をエンタープライズ管理設定で一元制御できるようになった。開発者ごとの環境変数設定が不要になり、ガバナンスとオブザーバビリティが向上。

## 詳細

エンタープライズ管理設定の `telemetry` ブロックを通じて、VS Code の Copilot Chat 拡張機能と Copilot CLI のエージェントホストプロセスに対して OpenTelemetry エクスポートを設定できる。

### 管理者が制御可能な項目

- OTLP エクスポートエンドポイントおよびトランスポートプロトコル（`otlp-http` / `otlp-grpc`）
- OTel サービス名とリソース属性
- エクスポーターヘッダー（コレクターの認証トークンなど）
- プロンプト・レスポンス・ツールコンテンツのキャプチャ有無と開発者による変更可否

### 設定の優先順位

管理対象の値は常に優先され、環境変数やユーザー設定を上書きする。設定は以下のチャネルから配信可能：

- ネイティブ MDM（Windows レジストリまたは macOS マネージド設定）
- サーバー管理設定（認証済み GitHub アカウントから解決）
- ファイルベースの `managed-settings.json`

### セキュリティ

管理対象のエクスポーターヘッダーは Copilot Chat 拡張機能の OTLP エクスポーターにのみ適用され、エージェントホストが生成するツールサブプロセスには環境変数として渡されない。

## 参考リンク

- [Enterprise-managed OpenTelemetry export for VS Code and CLI](https://github.blog/changelog/2026-07-08-enterprise-managed-opentelemetry-export-for-vs-code-and-cli/)
- [Configure telemetry export with OpenTelemetry](https://code.visualstudio.com/docs/enterprise/ai-settings#_configure-telemetry-export-with-opentelemetry)
- [Monitor agent usage with OpenTelemetry](https://code.visualstudio.com/docs/agents/guides/monitoring-agents)
