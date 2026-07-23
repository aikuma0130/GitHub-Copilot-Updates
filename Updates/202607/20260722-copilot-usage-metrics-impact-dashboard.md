# Copilot 使用メトリクスのインパクトダッシュボードが新登場

## 日付

2026-07-22

## ステータス

GA

## 概要

エンタープライズ管理者・組織オーナー向けに、Copilot の利用深度と影響を可視化する新しいインパクトダッシュボードが追加。AI 採用フェーズ別のコホート分析により、単なるアクティブユーザー数を超えた活用状況の把握が可能に。

## 詳細

### 主な機能

- **採用コホート**: ユーザーを AI 採用フェーズ別に分類し、フェーズごとのカードを表示
  - **Phase 1（コードファースト）**: 主にインラインコード補完を利用
  - **Phase 2（エージェントファースト）**: エージェント機能（Copilot Chat など）を活用
  - **Phase 3（マルチエージェント）**: 複数エージェントや Copilot アプリを使用
  - **パッシブ**: ライセンスを付与されているが未使用のユーザー
- **コホートメトリクス**: 各フェーズカードに以下を表示
  - ユーザーあたりの月間平均マージ PR 数
  - PR マージ速度の中央値
  - フェーズ内のユーザー数と全体に占める割合
  - ユーザーあたりの1日の平均コード行数
- **採用乗数（Adoption Multiplier）**: パッシブコホートとアクティブユーザー平均のスループット・速度比較
- **トレンド**: コホートの成長と PR スループットの6ヶ月チャート
- **推奨次ステップ**: より深い採用フェーズへの移行に向けた管理者向けアクションガイダンス

### 利用対象

- Copilot 使用メトリクスにアクセス可能なエンタープライズ管理者および組織オーナー

### 技術的詳細

- コホート割り当ては Copilot 使用メトリクス API の `ai_adoption_phase` 分類を使用
- 直近28日間のローリングウィンドウに基づくプロダクト使用状況で判定

## 参考リンク

- [New Copilot usage metrics impact dashboard](https://github.blog/changelog/2026-07-22-new-copilot-usage-metrics-impact-dashboard/)
- [Copilot usage metrics](https://docs.github.com/copilot/concepts/copilot-usage-metrics)
- [Copilot usage metrics API adds cohorts for AI adoption](https://github.blog/changelog/2026-05-29-copilot-usage-metrics-api-adds-cohorts-for-ai-adoption/)
