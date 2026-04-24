# JetBrains IDE 向け Copilot にインラインエージェントモードなど多数の改善

## 日付

2026-04-24

## ステータス

Public Preview / GA

## 概要

JetBrains IDE 向け GitHub Copilot にインラインエージェントモード（パブリックプレビュー）、Next Edit Suggestions の強化、グローバル自動承認機能などが追加されました。

## 詳細

### 新機能

#### インラインエージェントモード（パブリックプレビュー）

エージェントモードの機能をインラインチャットで利用可能に。エディタから直接、チャットパネルに切り替えることなくより強力なコンテキスト対応の支援を受けられます。

- **アクセス方法**: Shift+Ctrl+I（Windows）/ Shift+Cmd+I（Mac）でインラインチャットを開き、エージェントモードに切り替え
- **注意**: Copilot Business/Enterprise のユーザーは管理者が「Editor preview features」ポリシーを有効にする必要があります

#### Next Edit Suggestions の強化

- **インライン編集プレビュー**: 提案された変更をエディタ内で直接確認してから適用可能
- **遠距離編集**: 数画面先の編集候補にガターのクイック方向インジケーターで直接ジャンプ可能

#### グローバル自動承認と詳細制御

- **グローバル自動承認**: 全ワークスペースの全ツールコールを自動承認（セキュリティリスクを理解した上で有効化）
- **詳細制御**: ルールでカバーされないターミナルコマンドやファイル編集のデフォルト自動承認動作を設定可能

### UX 改善

- チャットコンテキストがメッセージ送信後に自動リセット
- 大規模な会話のチャット履歴レンダリングパフォーマンス向上
- インラインコードレビューパネルの自動リサイズ対応
- ログインフローの改善

### 品質改善

- チャットスピナー動作の改善
- Esc キーの動作改善
- Configure Tools ウィンドウの状態管理改善
- UI フリーズ処理と安定性の向上

## 参考リンク

- [Inline agent mode in preview and more in GitHub Copilot for JetBrains IDEs](https://github.blog/changelog/2026-04-24-inline-agent-mode-in-preview-and-more-in-github-copilot-for-jetbrains-ides)
- [GitHub Copilot for JetBrains IDEs プラグイン](https://plugins.jetbrains.com/plugin/17718-github-copilot--your-ai-pair-programmer/versions)
- [フィードバックリポジトリ](https://github.com/microsoft/copilot-intellij-feedback/issues)
