# Copilot Code Review: エージェントスキルと MCP が GA に

## 日付

2026-07-29

## ステータス

GA

## 概要

Copilot Code Review のエージェントスキルおよび MCP サーバー連携が、Copilot Pro、Pro+、Business、Enterprise の全ユーザー向けに正式 GA となった。チームのツール・コーディング規約・外部コンテキストをコードレビューに直接統合可能に。

## 詳細

### 含まれる機能

- **エージェントスキル**: `.github/skills` 配下のサブディレクトリに `SKILL.md` ファイルを追加することで、Copilot Code Review がチームの内部ツールやコーディング規約をレビュー時に参照・実行可能に。リポジトリまたは組織固有のコンテキストと指示でレビューの分析を拡張できる。
- **MCP サーバー接続**: チームが既に利用しているサードパーティプラットフォーム（イシュートラッカー、ドキュメントシステム、サービスカタログ等）からコンテキストをレビューに直接取り込み可能。
  - Copilot Code Review による MCP ツール呼び出しは読み取り専用に制限される。
  - Copilot クラウドエージェント用に設定済みの MCP 構成は、自動的に Code Review にも適用される。GitHub MCP と Playwright MCP はデフォルトで有効。

### 新機能

- **スキルおよび MCP コメントの帰属表示**: エージェントスキルまたは MCP コンテキストを使用して生成されたコメントには、その旨が表示されるようになった。

### 始め方

- パブリックプレビュー中にエージェントスキルまたは MCP サーバーを設定済みの場合、変更は不要。
- **MCP サーバー**: リポジトリ設定 → **Copilot** → **MCP servers** で構成を追加。認証トークンは **Secrets and variables** → **Agents** に保存。
- **エージェントスキル**: `.github/skills` 配下にスキル固有のディレクトリを作成し、`SKILL.md` ファイルを追加。

## 参考リンク

- [Copilot code review: Agent skills and MCP now generally available](https://github.blog/changelog/2026-07-29-copilot-code-review-agent-skills-and-mcp-now-generally-available/)
- [Shape Copilot code review around your team（パブリックプレビュー時の発表）](https://github.blog/changelog/2026-06-02-shape-copilot-code-review-around-your-team/)
- [エージェントスキルのドキュメント](https://docs.github.com/copilot/concepts/agents/about-agent-skills)
- [MCP サーバー設定例](https://docs.github.com/copilot/how-tos/copilot-on-github/customize-copilot/configure-mcp-servers#example-configurations)
