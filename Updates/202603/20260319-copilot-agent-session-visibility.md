# Copilot Coding Agent セッションの可視性を向上

## 日付

2026-03-19

## ステータス

Improvement

## 概要

Copilot Coding Agent のセッションログが改善。ビルトイン/カスタムセットアップステップの進捗表示とサブエージェント作業の折りたたみ表示に対応。

## 詳細

Copilot Coding Agent のセッションログに以下の改善が加えられました：

- **ビルトインセットアップステップの可視化**: リポジトリのクローンやエージェントファイアウォールの起動など、タスク開始前の準備ステップの進捗を表示
- **カスタムセットアップステップの可視化**: `copilot-setup-steps.yml` で定義したカスタムステップの出力をセッションログに表示
- **サブエージェントの可視化**: サブエージェントに作業を委任した際、そのアクティビティをデフォルトで折りたたみ表示し、現在の作業内容を HUD で表示

## 参考リンク

- [More visibility into Copilot coding agent sessions](https://github.blog/changelog/2026-03-19-more-visibility-into-copilot-coding-agent-sessions)
