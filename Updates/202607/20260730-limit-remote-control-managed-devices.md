# リモートコントロールをマネージドデバイスに制限

## 日付

2026-07-30

## ステータス

GA

## 概要

エンタープライズおよび組織が、リモートコントロール対象の Copilot セッションをホストできるデバイスを制限可能に。新しい `remoteControl` エンタープライズ管理設定により、デバイス単位のきめ細かなアクセス制御を実現。

## 詳細

### 新しい管理設定

- **`remoteControl` 設定**: エンタープライズ管理設定として追加。マネージドデバイスでのリモートコントロールの動作を詳細に定義可能。
  - `requireSSO`: SSO 認証を強制
  - `disabled`: リモートコントロールを完全にブロック
  - `enabled`: 制限なしで許可

### 既存ポリシーとの連携

- 既存のエンタープライズポリシー（ユーザーへのリモートコントロール利用可否全般を制御）と組み合わせて、広範なアクセスからデバイス単位の制限まで階層的な制御が可能。

### デプロイ方法

- **サーバー管理（`.github-private` リポジトリ）**: エンタープライズ内のユーザーアカウントに適用。
- **MDM 管理**: 特定のデバイスに適用。マネージドマシンでのポリシー適用に最適。
- **ファイルベース**: ファイルを受信する任意のマシンに適用。

### `copilot-settings.json` への追加

`remoteControl` キーを `copilot-settings.json` に追加することでも設定可能。

## 参考リンク

- [Limit remote control to managed devices](https://github.blog/changelog/2026-07-30-limit-remote-control-to-managed-devices)
- [エンタープライズ管理設定ドキュメント](https://docs.github.com/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/configure-enterprise-managed-settings)
