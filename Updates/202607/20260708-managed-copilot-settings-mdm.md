# MDM 経由で Copilot 管理設定をデバイスにデプロイ可能に

## 日付

2026-07-08

## ステータス

GA

## 概要

エンタープライズ管理者がネイティブ MDM（Intune、Jamf、Group Policy）やファイルベースの設定を通じて、Copilot の管理設定を VS Code および Copilot CLI に直接デプロイ可能になった。既存のエンドポイント管理ツールで Copilot ガバナンスを強制できる。

## 詳細

### 配信チャネル

3つのチャネルから管理設定を配信可能（すべて同じキーと値を使用）:

1. **ネイティブ MDM**: OS レベルの管理設定を読み取り
   - Windows: `HKEY_LOCAL_MACHINE\SOFTWARE\Policies\GitHubCopilot` レジストリキー
   - macOS: `com.github.copilot` ドメインの管理設定
2. **ファイルベース**: 所定パスの `managed-settings.json` ファイルを読み取り
   - macOS: `/Library/Application Support/GitHubCopilot/managed-settings.json`
   - Windows: `%ProgramFiles%\GitHubCopilot\managed-settings.json`
   - Linux: `/etc/github-copilot/managed-settings.json`
3. **サーバー管理**: `.github-private` リポジトリの `managed-settings.json` から解決

### 優先順位

複数チャネルが設定を提供する場合、以下の順に最も優先度の高いものが適用:

1. ネイティブ MDM
2. サーバー管理
3. ファイルベース

### サポートされる設定キー

- `permissions.disableBypassPermissionsMode`
- `model`
- `enabledPlugins`
- `extraKnownMarketplaces`
- `strictKnownMarketplaces`
- `telemetry.*`（OpenTelemetry エクスポート設定）

## 参考リンク

- [Deploy managed Copilot settings via MDM in VS Code and CLI](https://github.blog/changelog/2026-07-08-deploy-managed-copilot-settings-via-mdm-in-vs-code-and-cli/)
- [Deploy Copilot managed settings (VS Code docs)](https://code.visualstudio.com/docs/enterprise/ai-settings#_deploy-copilot-managed-settings)
- [Configure enterprise managed settings](https://docs.github.com/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/configure-enterprise-managed-settings)
