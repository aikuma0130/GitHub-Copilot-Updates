# Copilot SDK がパブリックプレビューで利用可能に

## 日付

2026-04-02

## ステータス

Public Preview

## 概要

GitHub Copilot SDK がパブリックプレビューとして公開されました。Copilot のエージェント機能を独自のアプリケーション、ワークフロー、プラットフォームサービスに直接組み込むためのビルディングブロックを提供します。

## 詳細

Copilot SDK は、Copilot cloud agent や Copilot CLI を支える本番実績のあるエージェントランタイムと同じものを提供します。独自の AI オーケストレーション層を構築する代わりに、ツール呼び出し、ストリーミング、ファイル操作、マルチターンセッションを即座に利用できます。

### 5つの言語で利用可能

- **Node.js / TypeScript**: `npm install @github/copilot-sdk`
- **Python**: `pip install github-copilot-sdk`
- **Go**: `go get github.com/github/copilot-sdk/go`
- **.NET**: `dotnet add package GitHub.Copilot.SDK`
- **Java**: Maven 経由でインストール可能

### 主な機能

- **カスタムツールとエージェント**: ドメイン固有のツールをハンドラー付きで定義し、エージェントが呼び出しタイミングを判断。カスタムエージェントの構築も可能
- **きめ細かなシステムプロンプトのカスタマイズ**: `replace`、`append`、`prepend`、動的な `transform` コールバックでシステムプロンプトのセクションをカスタマイズ
- **ストリーミングとリアルタイムレスポンス**: トークンごとのストリーミングでレスポンシブな UX を実現
- **Blob 添付**: 画像、スクリーンショット、バイナリデータをディスク書き込みなしでインラインで送信
- **OpenTelemetry サポート**: W3C トレースコンテキスト伝播による分散トレーシングを全 SDK でサポート
- **パーミッションフレームワーク**: 承認ハンドラーで機密操作をゲート、読み取り専用ツールはパーミッション不要
- **Bring Your Own Key (BYOK)**: OpenAI、Azure AI Foundry、Anthropic の独自 API キーを使用可能

### 利用条件

- Copilot サブスクライバーおよび非サブスクライバー（Copilot Free を含む）で利用可能
- BYOK はエンタープライズ向けに対応
- 各プロンプトは Copilot サブスクライバーのプレミアムリクエストクォータに算入

## 参考リンク

- [Copilot SDK in public preview](https://github.blog/changelog/2026-04-02-copilot-sdk-in-public-preview)
- [Copilot SDK - GitHub](https://github.com/github/copilot-sdk)
