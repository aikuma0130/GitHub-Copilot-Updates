# コストセンターのユーザー別予算が課金 UI で設定可能に

## 日付

2026-07-07

## ステータス

GA

## 概要

エンタープライズ管理者がコストセンターのユーザーレベル予算を課金 UI から直接作成可能になった。これまで REST API でのみ利用可能だった機能が GUI でも利用可能に。

## 詳細

### 主な特徴

- エンタープライズチームまたは個別ユーザーをコストセンターに追加可能
- コストセンターに1つのユーザー別予算を設定すると、所属する全員に自動適用
- メンバーシップの変更に応じて予算カバレッジが自動同期
- チーム移動時に予算の再設定が不要

### 対象

- GitHub Enterprise Cloud で利用可能
- AI クレジットの使用量制御に対応

### メリット

- REST API を使わずに UI から直感的に予算管理が可能
- チーム変更時の運用負荷を軽減
- エンタープライズ全体のコスト管理を効率化

## 参考リンク

- [Per-user budgets for cost centers in the billing UI](https://github.blog/changelog/2026-07-07-per-user-budgets-for-cost-centers-in-the-billing-ui/)
- [Budgets for usage-based billing - GitHub Docs](https://docs.github.com/enterprise-cloud@latest/copilot/concepts/billing/budgets-for-usage-based-billing)
- [Control GitHub costs at scale - GitHub Docs](https://docs.github.com/enterprise-cloud@latest/billing/tutorials/control-costs-at-scale)
