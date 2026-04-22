# VS Code で BYOK（独自モデルキー）が利用可能に

## 日付

2026-04-22

## ステータス

GA

## 概要

Copilot Business および Enterprise ユーザーが、Visual Studio Code で独自の API キーを使用して外部モデルプロバイダーに接続できる BYOK（Bring Your Own Key）機能が利用可能になりました。

## 詳細

### BYOK の概要

BYOK を使用することで、チームは Anthropic、Gemini、OpenAI、OpenRouter、Azure などのプロバイダーの API キーを再利用し、VS Code Chat 内でそれらのモデルにアクセスできます。Ollama や Foundry Local を通じたローカルモデルの接続にも対応しています。

### 対応範囲

- VS Code Chat 内のすべての場所（ビルトインの plan エージェントやカスタムエージェントを含む）で BYOK モデルが利用可能
- コード補完には適用されません
- 使用量は選択したプロバイダーに直接課金され、GitHub Copilot のリクエストクォータにはカウントされません

### 設定方法

ポリシーはデフォルトで有効化されています。Organization メンバーはビルトインプロバイダーからモデルを追加するか、言語モデルプロバイダー拡張機能をインストールして利用できます。Organization 管理者は github.com の Copilot ポリシー設定から「Bring Your Own Language Model Key in VS Code」ポリシーを無効化できます。

## 参考リンク

- [Bring your own language model key in VS Code now available](https://github.blog/changelog/2026-04-22-bring-your-own-language-model-key-in-vs-code-now-available/)
