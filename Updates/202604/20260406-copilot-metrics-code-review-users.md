# Copilot 利用メトリクスにコードレビューのアクティブ・パッシブユーザー識別を追加

## 日付

2026-04-06

## ステータス

Release

## 概要

Copilot 利用メトリクスでコードレビュー（CCR）のアクティビティがアクティブとパッシブに区別されるようになり、Enterprise・Organization 管理者がユーザーのエンゲージメント状況をより詳細に把握できるようになりました。

## 詳細

Copilot 利用メトリクス API に、ユーザーレベルで Copilot コードレビュー（CCR）のアクティビティを示す2つの新しいフィールドが追加されました。

### 新しいフィールド

- **`used_copilot_code_review_active`**: ユーザーが意図的に Copilot コードレビューに関与した場合に `true` になります。具体的には以下のアクションが該当します：
  - PR に Copilot をレビュアーとしてアサイン
  - Copilot レビューの再リクエスト
  - CCR の提案を適用
- **`used_copilot_code_review_passive`**: リポジトリレベルのポリシーにより Copilot コードレビューが自動実行されたが、ユーザーがレビューに対話しなかった場合に `true` になります。

### ポイント

- 同一日にアクティブとパッシブの両方の CCR イベントがある場合、アクティブが優先されます。
- 日次レポートおよび28日間レポートの両方で確認可能です。
- `used_agent`（IDE エージェントモード）や `used_copilot_coding_agent`（CCA）と並んで、Copilot の各機能の採用状況を包括的に把握できます。

### 活用例

- **実際のエンゲージメントの測定**: 自動レビューされているだけのユーザーと、積極的にレビューを活用しているユーザーを区別できます。
- **導入成熟度の追跡**: 「リポジトリの100%が CCR でカバーされ、ユーザーの60%がアクティブに活用」といった詳細な分析が可能になります。

## 参考リンク

- [Copilot usage metrics now identify active and passive Copilot code review users](https://github.blog/changelog/2026-04-06-copilot-usage-metrics-now-identify-active-and-passive-copilot-code-review-users)
- [Copilot Usage Metrics API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
- [Copilot メトリクスについてのドキュメント](https://docs.github.com/copilot/concepts/copilot-usage-metrics/copilot-metrics)
