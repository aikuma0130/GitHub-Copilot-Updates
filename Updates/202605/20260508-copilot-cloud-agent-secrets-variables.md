# Copilot Cloud Agent のシークレットと変数の柔軟な管理

## 日付

2026-05-08

## ステータス

GA

## 概要

Copilot Cloud Agent 向けのシークレットと変数がオーガニゼーションレベルで設定可能になりました。既存の Actions / Codespaces / Dependabot と並ぶ専用の「Agents」タイプとして管理でき、複数リポジトリへの一括展開が容易になります。

## 詳細

### 背景

これまで Copilot Cloud Agent にシークレットや変数を渡すには、各リポジトリの Actions 設定にある `copilot` 環境で個別に設定する必要がありました。共通設定（内部パッケージレジストリのトークンや MCP サーバー設定など）を多数のリポジトリに展開するのが困難でした。

### 新機能

Copilot Cloud Agent 専用の「Agents」シークレット・変数タイプが追加され、以下が可能になりました：

- **オーガニゼーションレベルでの設定**: シークレットと変数をオーガニゼーション全体で初めて一元管理し、任意のリポジトリ間で共有可能
- **専用の管理セクション**: リポジトリ設定に「Agents」専用セクションが追加され、Actions 設定と分離して管理可能
- **リポジトリ単位のアクセス制御**: Actions と同様に、各シークレット・変数にアクセスできるリポジトリを選択可能

### メリット

大規模な組織で Copilot Cloud Agent を利用する際に、リポジトリごとに設定を重複させる必要がなくなり、スケーラブルな運用が実現できます。

## 参考リンク

- [More flexible secrets and variables for Copilot cloud agent](https://github.blog/changelog/2026-05-08-more-flexible-secrets-and-variables-for-copilot-cloud-agent/)
- [Copilot Cloud Agent のシークレットと変数の設定ドキュメント](https://docs.github.com/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/configure-secrets-and-variables)
