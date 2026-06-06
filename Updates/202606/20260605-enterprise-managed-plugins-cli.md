# Copilot CLI のエンタープライズ管理プラグインがパブリックプレビュー

## 日付

2026-06-05

## ステータス

Public Preview

## 概要

エンタープライズ管理者が Copilot CLI のプラグインを一元配布・管理可能に。カスタムエージェントやスキルの組織全体への展開とガバナンス強化を支援。

## 詳細

エンタープライズ管理者が GitHub Copilot CLI ユーザー向けにプラグインを構成・配布できるようになった。

### 主な機能

- エンタープライズ全体のベースライン標準を設定し、すべてのユーザーの Copilot CLI クライアントで利用可能に
- プラグインマーケットプレースを `settings.json` ファイルで定義（`.github-private/.github/copilot/settings.json`）
- ユーザーが Copilot CLI で認証する際にプラグインを自動インストール
- カスタムエージェントやスキルの組織全体への共有

### メリット

- 開発者のオンボーディング改善とセットアップ時間の短縮
- hooks や MCP 設定を常時有効にすることでガバナンス戦略を強化
- 多くの拡張タイプをサポート

### 設定方法

Copilot Business または Copilot Enterprise でライセンスされたユーザーに対して、GitHub Copilot CLI がエンタープライズアカウントの設定を自動的に取得・適用する。カスタムエージェント用のソース組織を既に設定している場合、同じ `.github-private` リポジトリが使用される。

## 参考リンク

- [Enterprise-managed plugins in GitHub Copilot CLI are now in public preview](https://github.blog/changelog/2026-06-05-enterprise-managed-plugins-in-github-copilot-cli-are-now-in-public-preview/)
- [Enterprise managed client settings ドキュメント](https://docs.github.com/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/configure-enterprise-plugin-standards)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/178247)
