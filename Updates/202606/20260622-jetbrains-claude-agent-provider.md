# JetBrains IDE の新機能と Claude エージェントプロバイダープレビュー

## 日付

2026-06-22

## ステータス

Public Preview

## 概要

JetBrains IDE で Claude がエージェントプロバイダーとしてプレビュー利用可能に。Copilot CLI がデフォルトのエージェントハーネスとなり、メッセージのキューイング・ステアリングやデバッグログサマリービューなどの新機能が追加。

## 詳細

### Claude エージェントプロバイダー（プレビュー）

- JetBrains IDE 内で Claude をエージェントプロバイダーとして選択可能に
- 組織およびエンタープライズレベルのエージェントが JetBrains エコシステムで利用可能に
- エージェントモードでの柔軟なモデル選択が可能に

### Copilot CLI がデフォルトエージェントハーネスに

- JetBrains の Copilot 統合が、レガシーローカルハーネスに代わり Copilot CLI をデフォルトで使用
- VS Code や Web 版 Copilot と同じペースで新機能・モデルが提供可能に
- 既存のローカルエージェントセッションは自動変換され、ワークフローへの影響なし

### セッション管理機能の強化

- **メッセージのキューイング・ステアリング**: Copilot CLI セッション内で指示のキューイングとリアルタイム調整が可能に
- **エージェントデバッグログサマリービュー**: エージェント操作のデバッグログを要約表示する新ビューを追加

### その他の改善

- エージェント/Ask/編集モードでのコンテキスト一貫性の向上
- セッションのオープンおよびモード切り替え時の信頼性・パフォーマンス改善
- MCP レジストリの強化とエンタープライズ管理者向け許可リスト制御の追加

## 参考リンク

- [New features and Claude as agent provider preview in JetBrains IDEs](https://github.blog/changelog/2026-06-22-new-features-and-claude-as-agent-provider-preview-in-jetbrains-ides/)
- [GitHub Copilot for JetBrains is moving to Copilot CLI as the default agent harness](https://devblogs.microsoft.com/java/github-copilot-for-jetbrains-is-moving-to-copilot-cli-as-the-default-agent-harness/)
