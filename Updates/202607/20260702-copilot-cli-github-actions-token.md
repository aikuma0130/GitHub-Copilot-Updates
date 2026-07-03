# Copilot CLI が GitHub Actions で PAT 不要に

## 日付

2026-07-02

## ステータス

GA

## 概要

GitHub Actions で Copilot CLI を実行する際に、個人アクセストークン（PAT）が不要になり、組み込みの GITHUB_TOKEN で認証が可能に。セキュリティリスクの軽減と運用の簡素化を実現。

## 詳細

GitHub Copilot CLI を GitHub Actions 内で実行する際、ビルトインの `GITHUB_TOKEN` を使用して認証できるようになった。これにより、長期間有効な PAT の作成・管理が不要となり、大規模な自動化におけるセキュリティリスクと運用負荷が軽減される。

### 主な変更点

- ワークフローに `copilot-requests: write` パーミッションを付与するだけで利用可能
- 追加のシークレット設定は不要
- 組織所有のリポジトリでは、CLI が消費する AI クレジットは組織に直接課金される

### 設定方法

1. 組織の Copilot ポリシーで「Allow use of Copilot CLI billed to the organization」を有効にする（既存の「Copilot CLI」ポリシーが有効であれば、デフォルトで有効）
2. ワークフローに `copilot-requests: write` パーミッションを追加

### コスト管理

- ユーザーレベルの予算は組織直接課金時には適用されない
- コストセンターの設定やセッション制限を活用して支出を管理可能
- 組織の請求・使用状況ダッシュボードから消費量を監視可能

## 参考リンク

- [Copilot CLI no longer needs a personal access token in GitHub Actions](https://github.blog/changelog/2026-07-02-copilot-cli-no-longer-needs-a-personal-access-token-in-github-actions/)
- [Using Copilot CLI in GitHub Actions with GITHUB_TOKEN](https://docs.github.com/copilot/how-tos/copilot-cli/use-copilot-cli-in-actions)
