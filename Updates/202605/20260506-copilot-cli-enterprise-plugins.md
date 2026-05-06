# Copilot CLI エンタープライズ管理プラグイン（パブリックプレビュー）

## 日付

2026-05-06

## ステータス

Public Preview

## 概要

エンタープライズ管理者が GitHub Copilot CLI のプラグインを一元管理・配布できるようになりました。カスタムエージェント、スキル、フック、MCP 構成をエンタープライズ全体に展開でき、開発者のオンボーディング改善とガバナンス強化を実現します。

## 詳細

### 主な機能

- **プラグインの一元配布**: エンタープライズ管理者がプラグインを設定し、ライセンスを持つすべてのユーザーに自動配布
- **自動インストール**: ユーザーが Copilot CLI で認証する際にプラグインを自動的にインストール
- **ガバナンス強化**: フックや MCP 構成を常時有効化し、エンタープライズ全体のセキュリティポリシーを適用

### 設定方法

`.github-private/.github/copilot/settings.json` にプラグインマーケットプレイスを定義します。GitHub Copilot CLI が、Copilot Business または Copilot Enterprise のライセンスを持つユーザーに対して自動的にこれらの設定を適用します。

### 対象プラン

- Copilot Business
- Copilot Enterprise

### 前提条件

カスタムエージェント用のソース Organization が既に構成されている場合、プラグイン設定は同じ `.github-private` リポジトリを使用します。エンタープライズ設定の AI コントロール配下にある Agents ページで構成のアクティブ状態を確認できます。

## 参考リンク

- [Enterprise-managed plugins in GitHub Copilot CLI are now in public preview](https://github.blog/changelog/2026-05-06-enterprise-managed-plugins-in-github-copilot-cli-are-now-in-public-preview/)
- [Enterprise managed client settings docs](https://docs.github.com/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/configure-enterprise-plugin-standards)
- [Enterprise management concepts](https://docs.github.com/en/copilot/concepts/agents/enterprise-management)
