# GitHub Copilot が使用量ベース課金に移行

## 日付

2026-04-27

## ステータス

Announcement (2026年6月1日より適用)

## 概要

GitHub Copilot の全プランが 2026年6月1日より使用量ベース課金に移行します。プレミアムリクエスト単位（PRU）が廃止され、トークン消費量に基づく「GitHub AI クレジット」が導入されます。

## 詳細

### 主な変更点

- **PRU から AI クレジットへ**: プレミアムリクエスト単位に代わり、入力・出力・キャッシュトークンの消費量に基づく GitHub AI クレジットが導入されます。
- **プラン価格は据え置き**: Pro（$10/月）、Pro+（$39/月）、Business（$19/ユーザー/月）、Enterprise（$39/ユーザー/月）の価格は変更なし。月額と同額の AI クレジットが含まれます。
- **コード補完は対象外**: コード補完と Next Edit Suggestions は AI クレジットを消費せず、全プランに引き続き含まれます。
- **フォールバック廃止**: PRU 超過時の低コストモデルへのフォールバックは廃止され、利用可能なクレジットと管理者の予算設定に基づいて制御されます。
- **コードレビューは Actions 分数も消費**: プライベートリポジトリでの Copilot コードレビューは AI クレジットに加え GitHub Actions 分数も消費します。

### 個人プラン

- Copilot Pro: $10/月（$10 分の月間 AI クレジット含む）
- Copilot Pro+: $39/月（$39 分の月間 AI クレジット含む）
- 月額プランユーザーは 2026年6月1日に自動移行
- 年額プランユーザーはプラン満了まで既存の PRU ベース課金を継続

### ビジネス・エンタープライズ

- 移行初期（6〜8月）にプロモーション用の追加クレジットを自動付与
  - Business: $30/月の AI クレジット
  - Enterprise: $70/月の AI クレジット
- クレジットのプール利用が可能（組織全体で未使用分を共有）
- 管理者向けの予算コントロール機能（Enterprise・コストセンター・ユーザーレベルで設定可能）

### 移行支援

2026年5月初旬より「請求プレビュー」機能を提供し、移行前にコスト予測が可能になります。

## 参考リンク

- [GitHub Copilot is moving to usage-based billing](https://github.blog/news-insights/company-news/github-copilot-is-moving-to-usage-based-billing/)
- [使用量ベース課金への移行準備ドキュメント](https://docs.github.com/en/copilot/how-tos/manage-and-track-spending/prepare-for-your-move-to-usage-based-billing)
- [個人向け使用量ベース課金ドキュメント](https://docs.github.com/copilot/concepts/billing/usage-based-billing-for-individuals)
- [組織・エンタープライズ向けドキュメント](https://docs.github.com/copilot/concepts/billing/usage-based-billing-for-organizations-and-enterprises)
- [FAQ とコミュニティディスカッション](https://github.com/orgs/community/discussions/192948)
