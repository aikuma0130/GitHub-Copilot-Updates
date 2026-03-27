# Copilot 利用メトリクスで Coding Agent のアクティブユーザーを特定可能に

## 日付

2026-03-25

## ステータス

GA

## 概要

Copilot 利用メトリクスに、Copilot coding agent を積極的に利用しているユーザーを特定する `used_copilot_coding_agent` フィールドが追加されました。

## 詳細

Copilot 利用メトリクスで、どのユーザーが Copilot coding agent (CCA) アクティビティを行っているかを示すようになりました。

Enterprise および Organization の管理者は、日次および28日間レポートで CCA を積極的に使用しているユーザーを特定できます。API レスポンスでは、ユーザーレベルの `used_copilot_coding_agent` フィールドで確認できます。

IDE エージェントモードの使用（`used_agent`）と Copilot coding agent の使用（`used_copilot_coding_agent`）を区別することで、より明確な導入状況の把握が可能です。

## 参考リンク

- [Copilot usage metrics now identify active Copilot coding agent users](https://github.blog/changelog/2026-03-25-copilot-usage-metrics-now-identify-active-copilot-coding-agent-users)
