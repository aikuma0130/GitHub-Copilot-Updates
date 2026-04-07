# Copilot CLI が BYOK およびローカルモデルに対応

## 日付

2026-04-07

## ステータス

Release

## 概要

GitHub Copilot CLI で独自のモデルプロバイダーの接続やローカルモデルの実行が可能になり、エアギャップ環境での利用や LLM コストの直接管理が実現しました。

## 詳細

GitHub Copilot CLI に Bring Your Own Key（BYOK）機能とローカルモデル対応が追加され、GitHub がホストするモデルルーティングの代わりに独自のモデルプロバイダーやローカルモデルを利用できるようになりました。

### 任意のモデルプロバイダーの接続

環境変数を設定することで、Azure OpenAI、Anthropic、またはその他の OpenAI 互換エンドポイントを利用可能です。以下のプロバイダーに対応しています：

- **リモートサービス**: OpenAI、Azure OpenAI
- **ローカルモデル**: Ollama、vLLM、Foundry Local

### エアギャップ環境向けオフラインモード

`COPILOT_OFFLINE=true` を設定することで、GitHub サーバーへの通信を完全に遮断できます。オフラインモードではテレメトリが無効化され、CLI は設定されたプロバイダーのみと通信します。ローカルモデルと組み合わせることで、完全にエアギャップされた開発ワークフローが可能です。

### GitHub 認証がオプション化

独自のモデルプロバイダーを使用する場合、GitHub 認証は不要です。プロバイダーの認証情報のみですぐに利用開始できます。GitHub にサインインした場合は、`/delegate`、GitHub Code Search、GitHub MCP サーバーなどの追加機能も利用可能になります。

### 注意事項

- モデルは**ツール呼び出し**と**ストリーミング**に対応している必要があります。最良の結果を得るには、128k トークン以上のコンテキストウィンドウを持つモデルが推奨されます。
- 組み込みサブエージェント（explore、task、code-review）はプロバイダー設定を自動的に継承します。
- プロバイダー設定が無効な場合、GitHub ホストモデルへのサイレントフォールバックは行わず、実行可能なエラーメッセージを表示します。
- `copilot help providers` でターミナル内から設定手順を確認できます。

## 参考リンク

- [Copilot CLI now supports BYOK and local models](https://github.blog/changelog/2026-04-07-copilot-cli-now-supports-byok-and-local-models)
- [Using your own LLM models in GitHub Copilot CLI](https://docs.github.com/copilot/how-tos/copilot-cli/customize-copilot/use-byok-models)
- [Running in offline mode](https://docs.github.com/copilot/how-tos/copilot-cli/customize-copilot/use-byok-models#running-in-offline-mode)
- [Unauthenticated use](https://docs.github.com/copilot/how-tos/copilot-cli/set-up-copilot-cli/authenticate-copilot-cli#unauthenticated-use)
