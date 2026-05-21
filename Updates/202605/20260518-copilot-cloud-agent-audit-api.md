# Copilot Cloud Agent の構成を REST API で監査可能に

## 日付

2026-05-18

## ステータス

Public Preview

## 概要

新しい REST API エンドポイントにより、リポジトリの Copilot Cloud Agent 構成をプログラムから監査可能に。組織全体のセキュリティ姿勢を大規模に把握し、構成のドリフトを検出できる。

## 詳細

GitHub は「Get Copilot cloud agent configuration for a repository」REST API エンドポイントをパブリックプレビューとして公開した。

### 取得可能な構成情報

- MCP サーバー構成
- 有効化されている Copilot ツール
- GitHub Actions ワークフローポリシー
- ファイアウォール構成

### ユースケース

- 多数のリポジトリにまたがる Copilot Cloud Agent 設定のインベントリ作成
- 構成ドリフトの検出とフラグ付け
- 内部運用レポートの自動生成
- セキュリティ・ガバナンスチームによるコンプライアンス確認

従来は GitHub UI での手動スポットチェックが必要だったが、本 API によりスクリプトベースでの監査が可能となり、特に規制対象や業務上重要なリポジトリの運用成熟度が向上する。

## 参考リンク

- [Audit repository Copilot cloud agent configuration via the REST API](https://github.blog/changelog/2026-05-18-audit-repository-copilot-cloud-agent-configuration-via-the-rest-api)
