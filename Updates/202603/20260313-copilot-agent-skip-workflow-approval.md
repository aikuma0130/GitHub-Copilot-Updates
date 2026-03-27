# Copilot Coding Agent の Actions ワークフロー承認をオプションでスキップ可能に

## 日付

2026-03-13

## ステータス

Improvement

## 概要

Copilot Coding Agent が PR を作成した際の GitHub Actions ワークフロー承認をスキップする新しいリポジトリ設定を追加。デフォルトは承認必須のまま。

## 詳細

Copilot Coding Agent が PR を作成またはプッシュした際、外部コントリビュータと同様に扱われ、GitHub Actions ワークフローは人間の承認まで実行されません。新しいリポジトリ設定により、管理者はこの承認をスキップしてワークフローを即時実行させることが可能になりました。

デフォルトでは引き続き承認が必要です。セキュリティリスクを理解した上でフィードバックループを高速化したいリポジトリ向けのオプションです。

## 参考リンク

- [Optionally skip approval for Copilot coding agent Actions workflows](https://github.blog/changelog/2026-03-13-optionally-skip-approval-for-copilot-coding-agent-actions-workflows)
