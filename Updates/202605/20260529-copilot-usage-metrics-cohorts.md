# Copilot 使用量メトリクス API に AI 導入フェーズ（コホート）が追加

## 日付

2026-05-29

## ステータス

GA

## 概要

Copilot 使用量メトリクス API がユーザーを AI 導入フェーズ（コホート）に分類する機能を追加。単純なアクティブユーザー数を超えて、組織内での Copilot 活用の成熟度を可視化・追跡可能に。

## 詳細

### 新機能

ユーザーレベルレポートに `ai_adoption_phase` フィールドが追加され、エンタープライズ・組織レベルレポートには `totals_by_ai_adoption_phase` 配列が追加された。各ユーザーは過去28日間のローリングウィンドウにおける Copilot 利用パターンに基づき、以下の4フェーズに分類される：

- **Phase 0 — No cohort**: いずれのフェーズのエンゲージメント基準も満たさないユーザー
- **Phase 1 — Code first**: コード補完や IDE エージェントモードを利用しているユーザー
- **Phase 2 — Agent first**: GitHub ベースのエージェントサーフェス（Cloud Agent、Code Review、Copilot CLI）のいずれか1つを利用しているユーザー
- **Phase 3 — Multi-agent**: 2つ以上の GitHub ベースのエージェントサーフェス、または GitHub Copilot アプリを利用しているユーザー

### フェーズごとの集計メトリクス

- エンゲージユーザー数（28日間で2日以上の利用基準）
- ユーザー発信インタラクション平均
- コード生成・受容アクティビティ平均
- 追加・削除行数平均
- PR 作成・マージ・レビュー数平均
- マージまでの中央値時間平均

集計メトリクスはフェーズ内のユーザーあたりの**平均値**として報告される。

### 活用ポイント

- **成熟度ストーリーの可視化**: 単純なアクティブユーザー数を超えて、開発者が実際にどの Copilot 機能を採用しているかを把握可能
- **コホート進捗の追跡**: コード補完中心の利用からエージェント型・マルチエージェント型ワークフローへのユーザー成長を追跡
- **イネーブルメントの最適化**: 最大の改善機会があるフェーズにトレーニングやドキュメントを集中投下

### 注意事項

- エンタープライズ管理者および組織オーナーが REST API 経由で利用可能
- チームフィルターと組み合わせてさらに細かい粒度で分析可能

## 参考リンク

- [Copilot usage metrics API adds cohorts for AI adoption](https://github.blog/changelog/2026-05-29-copilot-usage-metrics-api-adds-cohorts-for-ai-adoption/)
- [Copilot usage metrics ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
