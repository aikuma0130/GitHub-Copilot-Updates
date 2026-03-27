# Copilot 使用メトリクスが Coding Agent アクティブユーザーを識別

## 日付

2026-03-25

## ステータス

Improvement

## 概要

使用メトリクスに `used_copilot_coding_agent` フィールドが追加。IDE のエージェントモードと Coding Agent の使用状況を区別可能に。

## 詳細

Copilot 使用メトリクスで、Copilot Coding Agent のアクティビティを持つユーザーを識別できるようになりました。API レスポンスの `used_copilot_coding_agent` フィールドにより、日次および28日レポートで Coding Agent のアクティブユーザーを確認できます。

- IDE エージェントモード使用（`used_agent`）と Coding Agent 使用（`used_copilot_coding_agent`）を区別
- Issue への Copilot アサインや PR コメントでの `@copilot` タグによるセッション開始を追跡

## 参考リンク

- [Copilot usage metrics now identify active Copilot coding agent users](https://github.blog/changelog/2026-03-25-copilot-usage-metrics-now-identify-active-copilot-coding-agent-users)
