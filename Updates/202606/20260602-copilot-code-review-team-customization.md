# Copilot Code Review をチームに合わせてカスタマイズ可能に

## 日付

2026-06-02

## ステータス

Public Preview

## 概要

Copilot Code Review にエージェントスキル・MCP サポートと新しい Medium 分析ティアが追加。チームのツールや基準に合わせたレビューのカスタマイズと、変更の複雑さに応じたレビュー深度の調整が可能に。

## 詳細

### エージェントスキルと MCP サポート

レビュアーが必要とする情報の多くは diff 以外のツールに存在する。エージェントスキルと MCP によりそのコンテキストをレビューに統合：

- **カスタムエージェントスキル**: チームの内部ツールや標準をレビュー中に呼び出し
- **MCP サーバー接続**: イシュー追跡、ドキュメント、サービスカタログ、インシデントツールなどの外部システムからコンテキストを取得
- **構成可能な Actions ワークフロー**: レビューに使用するコンピュートと環境を制御
- **レビューとクラウドエージェント間の共有設定**: 一度の設定で両エージェントで一貫した動作

### Medium 分析ティア

- **Medium**: 複雑なロジック、セキュリティに敏感なコード、クロスサービスの変更を深く分析するための高推論モデルにルーティング
- **Low**: ドキュメントや小規模リポジトリなど、単純な作業向けの高速・低コストデフォルト
- 管理者がリポジトリごとに Low / Medium を設定可能
- Medium は Low より多くの AI Credits を消費（コスト表示あり）

### 設定方法

#### MCP サーバーの設定

1. リポジトリ設定 → **Copilot** → **MCP servers** で JSON MCP 設定を追加
2. リポジトリ設定 → **Secrets and variables** → **Agents** で認証トークンを設定

#### エージェントスキルの設定

1. `.github/skills` ディレクトリを作成
2. `code-review` などのサブディレクトリを作成
3. `SKILL.md` ファイルにコンテキストと指示を記述

#### レビューティアの変更

リポジトリ設定 → **Copilot** → **Code review** → **Review effort level** でドロップダウンから選択

### 利用条件

Copilot Pro、Pro+、Business、Enterprise ユーザー向けパブリックプレビュー。Direct Org Billing でも非 Copilot ユーザーに有効化可能。

## 参考リンク

- [Shape Copilot code review around your team](https://github.blog/changelog/2026-06-02-shape-copilot-code-review-around-your-team/)
- [MCP 設定例](https://docs.github.com/copilot/how-tos/copilot-on-github/customize-copilot/configure-mcp-servers)
- [エージェントスキルについて](https://docs.github.com/copilot/concepts/agents/about-agent-skills)
- [Medium ティアレビュードキュメント](https://docs.github.com/copilot/concepts/agents/code-review)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/197304)
