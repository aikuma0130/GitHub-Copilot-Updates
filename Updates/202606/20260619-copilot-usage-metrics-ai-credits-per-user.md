# Copilot 使用状況メトリクス API にユーザーごとの AI クレジット消費量が追加

## 日付

2026-06-19

## ステータス

GA

## 概要

Copilot 使用状況メトリクス API に `ai_credits_used` フィールドが追加され、ユーザーごとの日次 AI クレジット消費量を追跡可能に。従量課金の詳細な可視化と予算管理を支援。

## 詳細

### 変更内容

- 使用状況メトリクス API のユーザーレベルレポートに `ai_credits_used` フィールドが新規追加
- エンタープライズおよび組織レベルの単日・28日レポートで利用可能
- 従量課金 API と同じデータソースを使用し、一貫性のあるデータを提供

### ユースケース

- チームやユーザーごとの AI クレジット消費量の把握
- 組織の利用状況と予算消化率の可視化
- Copilot がどこで最も価値を提供しているかの分析
- 使用量ベースの課金に対する予算計画の策定

### 注意事項

- このデータはメトリクス・分析用であり、直接的な課金計算には使用されない（課金は請求書ベース）
- GitHub の従量課金（AI Credits）モデルへの移行に伴い、より詳細な利用状況把握を可能にする機能追加

## 参考リンク

- [AI credits consumed per user now in the Copilot usage metrics API](https://github.blog/changelog/2026-06-19-ai-credits-consumed-per-user-now-in-the-copilot-usage-metrics-api/)
- [Copilot usage metrics API ドキュメント](https://docs.github.com/en/rest/copilot/copilot-usage)
