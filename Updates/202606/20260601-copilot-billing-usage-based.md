# GitHub Copilot の課金体系が従量課金（Usage-Based Billing）に移行

## 日付

2026-06-01

## ステータス

GA

## 概要

全 Copilot プランが GitHub AI Credits ベースの従量課金に移行。ユーザーレベルの予算管理機能の GA 化と、パワーユーザー向け Copilot Max プランの提供開始も同時発表。

## 詳細

### 従量課金の開始

2026年6月1日より、すべての Copilot プランが GitHub AI Credits の消費量に基づく従量課金方式に移行した。各プランには月次の含有利用量が設定されている。

- 含有 AI Credits を超過した場合、追加予算を設定することで月末に追加分が請求される
- 個人プランでは、利用パターン・課金履歴・アカウント認証ステータスに基づき追加 AI Credits の上限が設定される場合がある
- より多くの利用枠が必要な場合は上位プランへのアップグレードが推奨される

### Copilot Code Review 用デフォルト Actions ランナーの設定

Copilot Code Review が AI Credits に加えて Actions 分を消費するようになった。組織管理者は、全リポジトリで使用されるデフォルトランナーを組織レベルで一括設定可能に。

### ユーザーレベル予算管理（GA）

組織およびエンタープライズ向けに、ユーザーレベルの予算管理が一般提供開始。管理者は以下が可能に：

- 全ユーザーに対するユニバーサル予算の設定
- 特定ユーザーセットに対する予算オーバーライド
- 予算接近時のメール通知の受信
- AI Credits の場合、追加支出だけでなく総使用量を制御

### Copilot Max

既存の Student、Pro、Pro+ サブスクライバー向けに Copilot Max が提供開始。より多くの含有利用量と高い支出上限を備え、集中的なワークフローをサポートする。新規ユーザーの登録は数週間以内に開始予定。

### 新規登録の一時停止

Copilot Student、Pro、Pro+、Max プランへの新規登録は一時停止中。数週間以内に再開予定。

## 参考リンク

- [Updates to GitHub Copilot billing and plans](https://github.blog/changelog/2026-06-01-updates-to-github-copilot-billing-and-plans/)
- [GitHub Copilot is moving to usage-based billing](https://github.blog/news-insights/company-news/github-copilot-is-moving-to-usage-based-billing/)
- [個人向け従量課金ドキュメント](https://docs.github.com/copilot/concepts/billing/usage-based-billing-for-individuals)
- [組織・エンタープライズ向け従量課金ドキュメント](https://docs.github.com/copilot/concepts/billing/usage-based-billing-for-organizations-and-enterprises)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/197089)
