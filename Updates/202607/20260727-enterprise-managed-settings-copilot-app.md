# エンタープライズ管理設定が GitHub Copilot アプリとクラウドエージェントに適用

## 日付

2026-07-27

## ステータス

GA

## 概要

エンタープライズ管理設定（managed-settings.json）が GitHub Copilot アプリおよび Copilot クラウドエージェントにも適用されるようになり、全クライアントで一貫したガバナンスを実現。

## 詳細

### 概要

Copilot アプリとクラウドエージェントが、Copilot CLI や VS Code と同様にエンタープライズ管理設定の対象クライアントに追加された。`managed-settings.json` で定義したポリシーが全 Copilot サーフェスで一貫して適用される。

### 管理可能な設定項目

- 利用可能なプラグインの制御
- 開発者がインストールできるプラグインマーケットプレイスの制限
- 承認プロンプトのバイパス可否（コマンド実行、ファイルアクセス、URL フェッチ前）
- 新規会話でのオートモデル選択のデフォルト設定

### クライアントごとの適用範囲

- **Copilot アプリ**: プラグイン、マーケットプレイス、バイパスプロンプトの全設定が適用
- **Copilot クラウドエージェント**: プラグインとマーケットプレイスの設定が適用（バイパスプロンプト制御はインタラクティブクライアントのみ）

### 既存設定との互換性

既に Copilot CLI や VS Code 向けに `managed-settings.json` をデプロイしている場合、追加設定は不要。Copilot アプリは次回サインイン時またはアプリ再起動時に既存設定を自動的に読み込み、クラウドエージェントは次回タスク割り当て時に設定変更を反映する。

### 初回セットアップ手順

1. エンタープライズに `.github-private` リポジトリを作成・設定
2. `copilot/managed-settings.json` を作成または更新
3. JSON 形式でポリシーキーと値を記述し、デフォルトブランチにコミット・プッシュ

設定は約1時間以内に適用されるか、クライアント再起動・再サインイン時に即座に反映される。

## 参考リンク

- [Enterprise managed settings now apply to the GitHub Copilot app](https://github.blog/changelog/2026-07-27-enterprise-managed-settings-now-apply-to-the-github-copilot-app/)
- [エンタープライズ管理設定の構成ドキュメント](https://docs.github.com/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/configure-enterprise-managed-settings)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/199139)
