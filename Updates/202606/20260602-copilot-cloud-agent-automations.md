# Copilot クラウドエージェントでタスクのスケジュール・自動化が可能に

## 日付

2026-06-02

## ステータス

GA

## 概要

Copilot クラウドエージェントにオートメーション機能が追加。スケジュールまたはリポジトリイベントに応じて、エージェントタスクを自動実行可能に。

## 詳細

### 概要

新しい「オートメーション」機能により、Copilot クラウドエージェントがスケジュールやリポジトリイベントに応じて自動的に実行可能になった。手動入力なしで反復的なタスクをエージェントに委任できる。

### ユースケース例

- **イシューのトリアージ**: 新しいイシューを内容に基づいて `bug`、`enhancement`、`other` に自動ラベル付け
- **夜間のテスト修正**: 毎晩 `main` ブランチで失敗テストをチェックし、修正を試み、ドラフト PR を作成
- **週次リリースノート**: スケジュールに従ってリリースノートをドラフトし、PR を作成

### 対応リポジトリ

プライベートおよびインターナルリポジトリで利用可能。パブリックリポジトリへの対応は今後予定。

### 利用可能なプラン

- Copilot Pro、Pro+、Max、Business、Enterprise
- Business / Enterprise ユーザーは管理者によるクラウドエージェントポリシーの有効化が必要

### オートメーションの設定

github.com または GitHub Copilot アプリから作成可能：

- **名前**: オートメーションの識別名
- **プロンプト**: エージェントが実行すべき内容の説明
- **トリガー**: インターバル（時間ごと、日次、週次）、イシュー作成時、PR 作成・更新時
- **ツール**: エージェントが利用可能なツール（PR 作成、イシューラベル更新など）
- **モデル**: 使用するモデル（トークン使用量は標準の従量課金レートで課金）

## 参考リンク

- [Schedule and automate tasks with Copilot cloud agent](https://github.blog/changelog/2026-06-02-schedule-and-automate-tasks-with-copilot-cloud-agent/)
- [Copilot オートメーションドキュメント](https://gh.io/cca-automations-docs)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/197307)
