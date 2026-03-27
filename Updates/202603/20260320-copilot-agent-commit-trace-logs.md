# Copilot Coding Agent のコミットからセッションログをトレース可能に

## 日付

2026-03-20

## ステータス

Improvement

## 概要

Copilot Coding Agent のコミットに `Agent-Logs-Url` トレーラーが追加。コミットからセッションログへの永続的なリンクで監査性を向上。

## 詳細

Copilot Coding Agent のコミットメッセージに `Agent-Logs-Url` トレーラーが含まれるようになりました。これにより、エージェントが作成したコミットからフルセッションログへの永続的なリンクが提供されます。

コードレビュー時に Copilot が変更を行った理由を理解したり、監査目的で後からトレースしたりする際に活用できます。コミットの作者は Copilot で、タスクを開始した人間が co-author として記録されます。

## 参考リンク

- [Trace any Copilot coding agent commit to its session logs](https://github.blog/changelog/2026-03-20-trace-any-copilot-coding-agent-commit-to-its-session-logs)
