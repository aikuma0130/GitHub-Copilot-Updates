# 使用状況レポートで AI 導入フェーズ別のマージ合計数を追跡可能に

## 日付

2026-06-26

## ステータス

GA

## 概要

エンタープライズおよび組織レポートで、AI 導入フェーズごとのプルリクエストマージ合計数（total_pull_requests_merged）が追跡可能になった。従来のユーザー平均に加え、フェーズ間の絶対的なスループット比較が可能に。

## 詳細

### 新しいメトリクス

- `total_pull_requests_merged`: 特定の日に各 AI 導入フェーズのユーザーがマージしたプルリクエストの合計数
- 1日および28日ウィンドウのレポートで利用可能
- 既存の平均値メトリクスと同じアトリビューションロジックを使用

### AI 導入フェーズ

- **Phase 0**: 未エンゲージ
- **Phase 1**: コードファースト（コード補完や IDE エージェントモードを使用）
- **Phase 2**: エージェントファースト（単一のエージェント機能を使用）
- **Phase 3**: マルチエージェント（複数のエージェント機能や Copilot アプリを使用）

### 活用方法

- 各フェーズのマージ PR の割合を把握
- フェーズ間の絶対的なスループットを比較
- ユーザーが導入フェーズを進むにつれてスループットがどう変化するかを追跡

### 対象ユーザー

エンタープライズ管理者および組織オーナー（REST API 経由で Copilot 使用状況メトリクスにアクセス可能なユーザー）

## 参考リンク

- [Track total merges by adoption phase in enterprise and organization reports](https://github.blog/changelog/2026-06-26-track-total-merges-by-adoption-phase-in-enterprise-and-organization-reports/)
- [Copilot usage metrics documentation](https://docs.github.com/en/copilot/reference/copilot-usage-metrics/copilot-usage-metrics)
