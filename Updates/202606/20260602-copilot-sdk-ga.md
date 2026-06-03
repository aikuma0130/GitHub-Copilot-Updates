# Copilot SDK が一般提供開始

## 日付

2026-06-02

## ステータス

GA

## 概要

GitHub Copilot SDK が一般提供（GA）となり、Copilot のエージェントエンジンを独自のアプリケーションやサービスに安定した API で組み込めるようになった。

## 詳細

### 概要

GitHub Copilot SDK により、Copilot のエージェントランタイム（計画、ツール呼び出し、ファイル編集、ストリーミング、マルチターンセッション）にプログラムからアクセス可能になった。独自のオーケストレーション層を構築する必要がなくなる。

### 対応言語（6言語）

- **Node.js / TypeScript**: `npm install @github/copilot-sdk`
- **Python**: `pip install github-copilot-sdk`
- **Go**: `go get github.com/github/copilot-sdk/go`
- **.NET**: `dotnet add package GitHub.Copilot.SDK`
- **Rust**: `cargo add github-copilot-sdk`（GA で新規追加）
- **Java**: Maven / Gradle 経由（GA で新規追加）

### 主な機能

- **カスタムツールと MCP**: エージェントが自律的に呼び出すツールの登録、MCP サーバーへの接続、組み込みツールのオーバーライド
- **システムプロンプトのカスタマイズ**: ID、トーン、ツール指示、安全ルールなどを個別にカスタマイズ可能
- **OpenTelemetry トレーシング**: W3C トレースコンテキストの伝播
- **柔軟な認証**: GitHub OAuth、GitHub Apps、環境トークン、BYOK 対応
- **クラウド・リモートセッション**: クラウドバックのセッション作成やリモートセッション URL のオンデマンド生成
- **フックシステム**: ツール使用前後、セッション開始時、MCP ツール呼び出し時、権限要求時にインターセプト可能

### パブリックプレビューからの変更点

- Rust SDK が新規追加（Copilot CLI バイナリをデフォルトでバンドル）
- マルチクライアントワークフローのサポート強化
- スラッシュコマンドとインタラクティブ入力プロンプトが全 SDK で利用可能
- API サーフェスの安定化
- 接続診断の改善

### 料金と利用条件

Copilot Free を含むすべての GitHub Copilot サブスクライバーと、BYOK ユーザーが利用可能。

## 参考リンク

- [Copilot SDK is now generally available](https://github.blog/changelog/2026-06-02-copilot-sdk-is-now-generally-available/)
- [Copilot SDK リポジトリ](https://github.com/github/copilot-sdk)
- [Getting Started Guide](https://docs.github.com/copilot/how-tos/copilot-sdk/getting-started)
- [SDK ドキュメント](https://docs.github.com/copilot/how-tos/copilot-sdk)
