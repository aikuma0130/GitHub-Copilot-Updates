# Copilot Cloud Agent タスクを REST API で開始可能に

## 日付

2026-05-13

## ステータス

Public Preview

## 概要

Copilot Business / Enterprise ユーザーが新しい Agent tasks REST API を使用して、Copilot Cloud Agent のタスクをプログラムから開始できるようになった。カスタム自動化ワークフローへの組み込みが容易になり、大規模なリファクタリングやリポジトリセットアップなどの自動化が可能に。

## 詳細

### 新機能

Copilot Cloud Agent のタスクを REST API 経由でプログラム的に開始・追跡できる新しい Agent tasks REST API がパブリックプレビューとして提供開始された。

### ユースケース

- 複数リポジトリにまたがるリファクタリングやマイグレーションをスクリプトから一括実行
- 社内デベロッパーポータルからワンクリックで新規リポジトリをセットアップ
- リリースノートを含む新リリースを毎週自動準備

### 認証方法

- Personal Access Token（クラシック・Fine-grained）
- OAuth トークン

### 今後の対応予定

- GitHub App インストールアクセストークンのサポート
- Copilot Pro / Pro+ ユーザーへのアクセス開放

## 参考リンク

- [Start Copilot cloud agent tasks via the REST API](https://github.blog/changelog/2026-05-13-start-copilot-cloud-agent-tasks-via-the-rest-api/)
- [Agent tasks REST API ドキュメント](https://docs.github.com/rest/agent-tasks/agent-tasks?apiVersion=2026-03-10#start-a-task)
