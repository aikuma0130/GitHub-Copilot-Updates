# Copilot 使用メトリクス API にレビューサイクルとレビュー時間が追加

## 日付

2026-07-07

## ステータス

GA

## 概要

Copilot 使用メトリクス API の AI 採用フェーズ別集計に、PR のレビュー時間とレビューサイクル数の2つの新メトリクスが追加された。Copilot 採用度合いがレビュープロセスに与える影響を定量化できる。

## 詳細

### 新しいフィールド

`totals_by_ai_adoption_phase` ブレークダウンに以下の2つのフィールドが追加:

- **`avg_pull_requests_minutes_to_review`**: PR 作成から最初のレビューまでの中央値（分）
- **`avg_pull_requests_review_cycles`**: マージ前に PR が受けるレビュー提出数の中央値

両メトリクスは**マージ済み PR** にスコープされ、PR のマージ日に帰属する。レビューされたがマージされなかった PR はカウントされない。

### 重要性

レビュー遅延とレビューサイクル数はエンジニアリングスループットの先行指標となる。AI 採用フェーズ別に分類することで、Copilot 活用度が高いチームが PR レビューを迅速に完了し、より少ないレビューサイクルでイテレーションしているかを確認できる。

### 注意事項

- エンタープライズおよび組織の1日/28日レポートの両方に表示
- マージ済み PR にスコープされるため、実際にランディングした作業を反映
- フェーズ定義とコホート割り当ては変更なし

## 参考リンク

- [Add review cycles and time to adoption phases in the usage API](https://github.blog/changelog/2026-07-07-add-review-cycles-and-time-to-adoption-phases-in-the-usage-api/)
- [Copilot usage metrics API documentation](https://docs.github.com/rest/copilot/copilot-usage-metrics)
