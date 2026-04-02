# Copilot 利用メトリクスに Organization レポートのユーザー別 CLI アクティビティを追加

## 日付

2026-04-02

## ステータス

GA

## 概要

Copilot 利用メトリクスの Organization レポートにユーザー別の CLI アクティビティ詳細が追加され、管理者が個々の開発者の CLI 使用状況を把握できるようになりました。

## 詳細

エンタープライズレベル、ユーザーレベル、Organization レベルの CLI メトリクスリリースに続き、Organization レポートでのユーザー別 CLI 内訳が完成しました。

### 確認可能な情報

Organization 管理者は、1日および28日レポートで以下の情報を確認できます：

- 各ユーザーの CLI アクティビティの有無（`used_cli`）
- ユーザーごとの CLI セッション数とリクエスト数
- トークン使用量の合計（リクエストあたりの平均トークン数を含む）
- ユーザーごとの最新 CLI バージョン（アップグレード計画の支援用）

### 活用のポイント

- コマンドラインから Copilot を積極的に利用している開発者の特定と、有効化が必要な領域の把握
- ユーザーごとの消費パターンの理解によるコスト配分と展開計画の支援
- Organization 全体の CLI バージョン分布の追跡（サポート対象バージョンの確認）

## 参考リンク

- [Copilot usage metrics now includes per-user GitHub Copilot CLI activity in organization reports](https://github.blog/changelog/2026-04-02-copilot-usage-metrics-now-includes-per-user-github-copilot-cli-activity-in-organization-reports)
- [API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2026-03-10)
