# エンタープライズ管理設定で strictKnownMarketplaces が VS Code と Copilot CLI に対応

## 日付

2026-06-25

## ステータス

Public Preview

## 概要

エンタープライズ管理者が `strictKnownMarketplaces` 設定を使用して、VS Code と GitHub Copilot CLI で利用可能なプラグインマーケットプレースを厳格に制限可能に。承認済みソースからのみプラグインをインストールさせるガバナンス機能を提供。

## 詳細

### 概要

エンタープライズ管理環境において、`strictKnownMarketplaces` ポリシーが VS Code と GitHub Copilot CLI の両方でサポートされるようになった。これにより、管理者は組織で許可するプラグインマーケットプレースを明示的に制限できる。

### 主な機能

- **マーケットプレースの厳格な制限**: 承認済みのマーケットプレースからのみプラグインのインストールを許可
- **VS Code と Copilot CLI の両対応**: 統一されたポリシーで両環境を一元管理
- **既存のエンタープライズ管理設定との統合**: `.github-private/.github/copilot/settings.json` で設定

### ユースケース

- コンプライアンス要件に基づくプラグインソースの制御
- 未承認・悪意あるプラグインのインストール防止
- 開発環境のセキュリティ標準の統一

### 関連する既存機能

2026年6月5日にパブリックプレビューとして提供開始されたエンタープライズ管理プラグイン機能の拡張として位置づけられる。

## 参考リンク

- [Enterprise-managed settings now support strictKnownMarketplaces in VS Code and GitHub Copilot CLI](https://github.blog/changelog/2026-06-25-enterprise-managed-settings-now-support-strictknownmarketplaces-in-vs-code-and-github-copilot-cli/)
- [Enterprise-managed plugins in GitHub Copilot CLI are now in public preview](https://github.blog/changelog/2026-06-05-enterprise-managed-plugins-in-github-copilot-cli-are-now-in-public-preview/)
