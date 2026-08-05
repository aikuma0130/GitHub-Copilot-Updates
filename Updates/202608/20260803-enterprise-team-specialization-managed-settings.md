# エンタープライズチーム専門化による管理設定

## 日付

2026-08-03

## ステータス

GA

## 概要

エンタープライズ管理者がチームごとに管理設定をカスタマイズできるようになった。チームは定められた範囲内で Copilot をワークフローに適応させる柔軟性を持ちつつ、組織全体のガバナンスを維持できる。

## 詳細

`managed-settings.json` でキーを `overridable` に設定すると、チームごとに値を上書き可能。上書きされない場合はエンタープライズのデフォルト値にフォールバックする。

主な機能:
- **キーのオーバーライド指定**: `{ "overridable": true }` 構文でチーム別設定を許可
- **チームベースのプラグイン拡張**: `enabledPlugins` と `extraKnownMarketplaces` は加算方式で、エンタープライズのベースラインに追加される
- **設定ファイルのチームマッピング**: `team-mappings.json` で設定ファイルを複数チームに適用可能
- **エンタープライズ設定の優先**: オーバーライド不可のキーはコンプライアンス上ロックされたまま

対応クライアント: VS Code、Copilot CLI、Copilot App、Copilot Cloud Agent（Copilot Business/Enterprise ライセンスユーザー）。

## 参考リンク

- [Enterprise team specialization for managed settings](https://github.blog/changelog/2026-08-03-enterprise-team-specialization-for-managed-settings/)
- [Configuring enterprise managed settings](https://docs.github.com/enterprise-cloud@latest/copilot/reference/enterprise-managed-settings-reference#applying-different-settings-to-enterprise-teams)
