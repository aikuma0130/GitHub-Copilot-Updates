# Codex がエージェントプロバイダーとして JetBrains IDE で利用可能に

## 日付

2026-07-07

## ステータス

Public Preview

## 概要

Codex が JetBrains IDE で新しいエージェントプロバイダーとしてパブリックプレビューで利用可能に。カスタマイズエディターの拡張、Copilot CLI セッションの承認設定、カスタムモデルサポートなど多数のエージェント機能強化を含む。

## 詳細

### Codex エージェントプロバイダー（パブリックプレビュー）

Codex が JetBrains IDE 内で新しいエージェントプロバイダーとして選択可能に。タスクに最適なエージェントを IDE を離れることなく選択できる。

利用手順:
1. Codex CLI をマシンにインストール
2. Settings > Tools > GitHub Copilot > Chat で Codex を有効化し CLI パスを設定
3. Copilot Chat パネルのエージェントピッカーから Codex を選択

> Copilot Business / Enterprise ユーザーは、管理者がエディタープレビュー機能ポリシーを有効化する必要あり。

### エージェントカスタマイズの強化

- **Hooks サポート**: ローカルおよび Copilot CLI セッションの「Agent Customizations」で Hooks を管理可能に
- **MCP サーバー管理**: Copilot CLI セッション向けに MCP サーバーの管理が可能に。Browse Marketplace から閲覧、コマンド/HTTP タイプの追加、ステータス確認、開始/停止/再起動/アンインストールが可能。`.github/mcp.json` でワークスペースレベルの管理にも対応
- **AI によるカスタマイズファイル生成**: `/create-instruction`、`/create-prompt`、`/create-skill`、`/create-agent`、`/create-hook` コマンドでカスタマイズファイルをスキャフォールド可能

### Copilot CLI セッションの承認設定

Copilot CLI セッションの承認設定を構成可能に。チャット入力エリアの権限ドロップダウンから選択:

- **Default Approvals**: 設定済みの承認ポリシーに従い確認プロンプトを表示
- **Bypass Approvals**: すべてのツール呼び出しが確認なしで自動承認
- **Autopilot（プレビュー）**: すべてのツール呼び出しが自動承認され、質問にも自動応答してタスク完了まで反復

### Claude エージェントの権限モードとデバッグログ

Claude エージェントセッションで権限モード選択とデバッグログがサポート。

### カスタムモデルサポート

GitHub Copilot Business / Enterprise 管理者が設定したカスタムモデルが JetBrains IDE で自動的に利用可能に。

### その他の改善

- Inline Chat が GA に
- 使用量ベース課金のベストプラクティスのヒント追加
- Next Edit Suggestions (NES) のサジェスチョンキャッシュによる高速化
- ファイルウォッチャーのパフォーマンス改善とメモリ使用量削減
- BYOK セッションでのサブエージェント消費の修正

## 参考リンク

- [Codex as agent provider and agentic enhancements in JetBrains IDEs](https://github.blog/changelog/2026-07-07-codex-as-agent-provider-and-agentic-enhancements-in-jetbrains-ides/)
