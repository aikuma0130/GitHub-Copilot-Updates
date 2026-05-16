# JetBrains IDE 向け Copilot CLI エージェントと統合セッションビューの導入

## 日付

2026-05-13

## ステータス

Public Preview

## 概要

JetBrains IDE で Copilot CLI エージェントが利用可能になり、IDE から直接ターミナルベースのエージェントにタスクを委任できるようになった。また、すべてのエージェントセッションを一覧管理できる統合セッションビューも追加された。

## 詳細

### Copilot CLI エージェント（パブリックプレビュー）

JetBrains IDE からローカルで動作する Copilot CLI エージェントにタスクを委任できるようになった。エディタのコンテキストが自動的に接続される。

#### アイソレーションモード

エージェントは変更の適用方法を制御する2つのアイソレーションモードをサポート：

- **Worktree アイソレーション**: 別の Git ワークツリーでエージェントを実行し、レビューして適用するまで現在のブランチに影響しない
- **Workspace アイソレーション**: 現在のワークスペースに直接変更を適用し、アイソレーションが不要な場合の高速な反復を可能にする

### 統合セッションビュー

チャットウィンドウに統合セッションビューが追加され、すべてのエージェントセッションを一箇所で追跡可能に。各セッションにはタイトル、エージェントタイプ、経過時間、ステータスが表示される。エージェントタイプやステータスでフィルタリングも可能。

### Ask question ツール

Agent モードに Ask question ツールが追加され、追加情報が必要な場合にエージェントが明確化のための質問を行えるようになった。Agent モード、カスタムエージェント、サブエージェント、Copilot CLI エージェントで利用可能。

### グローバル `.agent.md` サポート

`~/.copilot/agents` 配下にグローバルレベルのカスタムエージェント定義が可能に。すべてのワークスペースで利用できるようになった。

### その他の改善

- GitHub Enterprise Server（GHES）のサインインフロー対応
- サブエージェントのレンダリングとスタイリングの改善
- コードレビュー適用動作の改善
- Edit モードのサポート終了

## 参考リンク

- [Introducing Copilot CLI agent and unified sessions view in GitHub Copilot for JetBrains IDEs](https://github.blog/changelog/2026-05-13-introducing-copilot-cli-agent-and-unified-sessions-view-in-github-copilot-for-jetbrains-ides/)
- [GitHub Copilot for JetBrains IDEs プラグイン](https://plugins.jetbrains.com/plugin/17718-github-copilot--your-ai-pair-programmer/versions)
