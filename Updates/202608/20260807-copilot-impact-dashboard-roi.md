# Copilot インパクトダッシュボードに ROI セクション追加

## 日付

2026-08-07

## ステータス

GA

## 概要

Copilot インパクトダッシュボードに「投資対効果（ROI）」セクションが追加され、Copilot の費用とプルリクエスト成果を直接比較できるようになった。

## 詳細

### 新機能

開発者を Copilot 活用度で 2 グループに分類し比較する 2 枚のカードが追加されました：

- **パッシブ/Phase 1 ユーザー**: チャットやコード補完を主に利用
- **Phase 2/Phase 3 ユーザー**: エージェントファーストの開発者

各カードに表示される指標：

- **コスト/開発者/月**: AI クレジット消費から算出した月額平均コスト
- **給与比率/月**: 上記コストの開発者報酬に対する割合
- **プルリクエスト/月**: 開発者あたりの月間平均プルリクエスト数

給与セレクターで報酬帯を選択すると、コスト関連指標が即座に再計算されます。

### その他の改善

- **採用コホートのユーザーカウント精度向上**: 28 日間レポートウィンドウ全体のアクティブユーザーを反映するように修正。週末や祝日の影響で数値が低くなる問題を解消。

### 対象ユーザー

- エンタープライズオーナーおよび請求管理者
- 組織オーナー
- `View Copilot Metrics` 権限を持つカスタムロールのユーザー

## 参考リンク

- [Copilot impact dashboard adds a return on investment section](https://github.blog/changelog/2026-08-07-copilot-impact-dashboard-adds-a-return-on-investment-section/)
- [Copilot impact dashboard documentation](https://docs.github.com/copilot/how-tos/administer-copilot/view-impact-dashboard)
