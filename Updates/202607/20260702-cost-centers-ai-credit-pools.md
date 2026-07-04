# コストセンターで AI クレジットプールが利用可能に

## 日付

2026-07-02

## ステータス

GA

## 概要

エンタープライズのコストセンターに AI クレジットプール（含有使用量上限）を設定可能に。各コストセンターが自身のライセンス分を超えて共有クレジットを消費することを防ぎ、チャージバック境界を維持する。

## 詳細

Copilot ライセンスに付属する月間含有 AI クレジットはエンタープライズ全体でプールされる。これまではコントロールがなく、1つのコストセンターが他のコストセンターのライセンスが支払ったクレジットを使い切る可能性があった。

### AI クレジットプールの仕組み

- コストセンターに割り当てられた Copilot Business / Enterprise ライセンスに基づき、使用上限が自動計算される
- ライセンスの追加・削除に応じて上限が自動調整される
- 上限到達時の動作を選択可能：追加使用をブロック、または追加課金として許可

### AI クレジットプールとバジェットの違い

- **AI クレジットプール**: 含有使用量プール（共有プール）からの使用を制限
- **コストセンターバジェット**: メーター課金フェーズ（含有量超過後の課金）を制限
- 両方を同じコストセンターに適用可能

### 利用条件

- GitHub Enterprise Cloud の Copilot Business / Copilot Enterprise で利用可能
- REST API 経由で設定可能（UI は近日提供予定）

## 参考リンク

- [Cost centers now support AI credit pools](https://github.blog/changelog/2026-07-02-cost-centers-now-support-included-usage-caps/)
- [Budgets for usage-based billing - GitHub Docs](https://docs.github.com/enterprise-cloud@latest/copilot/concepts/billing/budgets-for-usage-based-billing)
- [About cost centers - GitHub Docs](https://docs.github.com/enterprise-cloud@latest/billing/how-tos/products/use-cost-centers)
