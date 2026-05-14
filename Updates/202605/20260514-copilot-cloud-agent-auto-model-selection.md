# Copilot Cloud Agent が自動モデル選択に対応

## 日付

2026-05-14

## ステータス

GA

## 概要

Copilot Cloud Agent がモデルの自動選択（Auto）に対応。システムの健全性とモデルパフォーマンスに基づいて最適なモデルが自動的に選択され、通常のモデル乗数から 10% 割引が適用される。週次レート制限の影響も受けない。

## 詳細

### 新機能

モデルピッカーで「Auto」を選択すると、Copilot がシステムの健全性とモデルパフォーマンスに基づいて最適な利用可能モデルを自動的に選択する。

### メリット

- **コスト削減**: 通常のモデル乗数から 10% 割引が適用される
- **レート制限の回避**: 週次レート制限の影響を受けない
- **レイテンシの低減**: 最も健全なモデルが選択されるため、応答速度が向上
- **運用の簡素化**: ユーザーが手動でモデルを選択する必要がなくなる

### 適用範囲

- Copilot Cloud Agent のタスク実行時に利用可能
- 組織のポリシーで制限されたモデルや、プランで利用不可のモデルは自動選択の対象外

## 参考リンク

- [Copilot cloud agent supports auto model selection](https://github.blog/changelog/2026-05-14-copilot-cloud-agent-supports-auto-model-selection/)
- [About Copilot auto model selection](https://docs.github.com/copilot/concepts/auto-model-selection)
