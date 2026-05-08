# Copilot Code Review のコメントタイプが使用量メトリクス API に追加

## 日付

2026-05-08

## ステータス

GA

## 概要

Copilot 使用量メトリクス API に Code Review のサジェスションをコメントタイプ別に分類する新しいデータが追加されました。セキュリティやバグリスクなどのカテゴリごとにサジェスション数と適用数を確認できます。

## 詳細

### 新機能

Copilot 使用量メトリクス API の `pull_requests` 配下に、新しい `copilot_suggestions_by_comment_type` 配列が追加されました。Copilot Code Review が生成した各サジェスション（行単位のレビューコメント）について、コメントタイプ別の集計データを提供します。

### 提供されるデータ

| フィールド | 説明 |
|---|---|
| `comment_type` | Copilot がサジェスションに割り当てたカテゴリ（例: `security`, `bug_risk`） |
| `total_copilot_suggestions` | レポート期間中に投稿された当該タイプのサジェスション総数 |
| `total_copilot_applied_suggestions` | 開発者が適用したサジェスション数 |

### 利用可能なレポート形式

- 1日単位レポート
- 28日間ローリングウィンドウレポート
- エンタープライズおよびオーガニゼーションレベルで利用可能
- リポジトリレベルのドリルダウンは今後対応予定

### 活用例

- **Copilot が検出する問題の傾向把握**: どのカテゴリの問題が最も多く検出されているかを確認
- **開発者の採用率の測定**: タイプ別のサジェスション数と適用数を比較し、最も価値のある領域を特定
- **Code Review 全体像の把握**: 既存のユーザー数・PR メトリクスと組み合わせて、フィードバックの種類と採用率を可視化

### アクセス権限

エンタープライズ管理者およびオーガニゼーションオーナーが Copilot 使用量メトリクス REST API を通じて利用可能です。

## 参考リンク

- [Copilot code review comment types now in usage metrics API](https://github.blog/changelog/2026-05-08-copilot-code-review-comment-types-now-in-usage-metrics-api/)
- [Copilot 使用量メトリクス API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
