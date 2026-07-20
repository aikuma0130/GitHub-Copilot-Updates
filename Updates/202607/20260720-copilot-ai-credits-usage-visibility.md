# Copilot ユーザーが請求サイクルごとの AI クレジット使用量を確認可能に

## 日付

2026-07-20

## ステータス

GA

## 概要

Copilot Business / Enterprise ユーザーが、個別予算の設定有無にかかわらず、現在の請求サイクルで使用した AI クレジット数を確認可能に。使用状況の透明性が向上し、コスト管理が容易になった。

## 詳細

### 変更点

GitHub Copilot の使用量ページで、実際の AI クレジット消費量が表示されるようになった。

### 表示内容

- **個別予算が未設定の場合**: 現在の請求サイクルで使用した AI クレジットの合計が表示される
- **管理者が予算を設定している場合**: 予算総額に対する使用済みクレジット数が表示される

### 背景

従来は使用量が予算に対するパーセンテージとしてのみ表示されていた。個別予算が設定されていないユーザーにとっては月間使用量を把握する手段がなく、トークン消費のコンテキストを理解することが困難だった。

### 対象プラン

- Copilot Business
- Copilot Enterprise

## 参考リンク

- [Copilot users can now see AI credits used per billing cycle](https://github.blog/changelog/2026-07-20-copilot-users-can-now-see-ai-credits-used-per-billing-cycle/)
- [Budgets for usage-based billing](https://docs.github.com/enterprise-cloud@latest/copilot/concepts/billing/budgets-for-usage-based-billing)
