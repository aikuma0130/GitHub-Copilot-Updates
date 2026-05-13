# Copilot Code Review: コメント体験の改善

## 日付

2026-05-12

## ステータス

GA

## 概要

Copilot Code Review のコメントがスキャンしやすく、対応しやすくなりました。グループ化されたサジェスション、重大度レベル、更新されたサジェスト変更セット UI により、ノイズを削減し優先順位付けを支援します。

## 詳細

新しいプルリクエストエクスペリエンスにオプトインしているすべてのユーザーが利用可能です。

### 重大度レベルによる優先順位付け

コメントに重大度ラベルが付与されるようになり、どのサジェスションを優先的に対応すべきか判断しやすくなりました。重大度ラベルは Copilot Code Review コメントの右上に表示され、`High`、`Medium`、`Low` の3段階で分類されます。

### グループ化されたコメントによるノイズ削減

Copilot Code Review が同種のコメントをグループ化するようになりました。特に大規模なプルリクエストにおいて、フィードバックのレビューが容易になり、繰り返しが軽減されます。例えば、プルリクエスト内の複数箇所で変数名の改善を提案する場合、Copilot は一度だけ指摘を行います。

## 参考リンク

- [Copilot code review: Comment experience improvements](https://github.blog/changelog/2026-05-12-copilot-code-review-comment-experience-improvements)
