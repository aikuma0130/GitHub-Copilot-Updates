# Enterprise managed-settings.json が GA（一般提供開始）

## 日付

2026-07-01

## ステータス

GA

## 概要

GitHub Enterprise Cloud の管理者が `managed-settings.json` ファイルを通じて Copilot クライアント（VS Code、Copilot CLI）のガバナンスおよび拡張性設定を一元管理できるようになった。

## 詳細

GitHub Enterprise Cloud の顧客は、選択した組織の `.github-private` リポジトリに `managed-settings.json` ファイルを配置することで、AI に関するガバナンスと拡張性のフローを定義できる。この設定はユーザーのローカル設定よりも優先され、認証時にフェッチされて1時間ごとに更新される。

### サポートされるキー

- `extraKnownMarketplaces`
- `enabledPlugins`
- `strictKnownMarketplaces`
- `disableBypassPermissionsMode`
- `model`

### サポートされるクライアント

VS Code および Copilot CLI で、Copilot Business または Copilot Enterprise ライセンスを持つユーザーに適用される。

### セットアップ方法

1. エンタープライズ設定の AI Controls タブでソース組織を選択
2. ソース組織の `.github-private` リポジトリに `copilot/managed-settings.json` を作成
3. サポートされるキーと値を追加してデフォルトブランチにコミット

## 参考リンク

- [Enterprise managed-settings.json is generally available](https://github.blog/changelog/2026-07-01-enterprise-managed-settings-json-is-generally-available/)
- [Configure enterprise managed settings](https://docs.github.com/enterprise-cloud@latest/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/configure-enterprise-managed-settings)
