# エージェントワークフローでパーソナルアクセストークンが不要に

## 日付

2026-06-11

## ステータス

GA

## 概要

GitHub Copilot のエージェントワークフローで、パーソナルアクセストークン（PAT）の手動管理が不要になり、GitHub Actions 組み込みの `GITHUB_TOKEN` で認証可能に。セキュリティリスクの軽減と設定の簡素化を実現。

## 詳細

### 主な変更点

- **PAT 不要**: エージェントワークフローが GitHub Actions の組み込み `GITHUB_TOKEN` を使用して認証するようになり、長期間有効な PAT の作成・管理・ローテーションが不要に。
- **組織レベルの課金**: 組織所有リポジトリでエージェントワークフローを実行した場合、消費された AI クレジットは組織に直接請求される。

### 設定方法

1. Copilot ポリシー設定で「Allow use of Copilot CLI billed to the organization」を有効化（Copilot CLI ポリシーが既にオンの場合はデフォルトで有効）
2. ワークフローのマークダウンフロントマターの permissions セクションに `copilot-requests: write` を追加
3. 最新の Agentic Workflows CLI にアップグレード（`gh extension upgrade aw`）

### コスト管理

- 組織レベルでの課金のため、個人ユーザー予算は適用されない
- コストセンターおよびグループ/組織ごとの予算設定で管理可能
- ワークフロー実行ごとのトークン使用量の監視・上限設定が可能

### 対象プラン

Free、Pro、Pro+、Business、Enterprise の全プランで利用可能。

## 参考リンク

- [Agentic workflows no longer need a personal access token](https://github.blog/changelog/2026-06-11-agentic-workflows-no-longer-need-a-personal-access-token/)
