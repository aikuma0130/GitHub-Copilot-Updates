# サードパーティコーディングエージェントのセキュリティ検証が一般提供開始

## 日付

2026-06-09

## ステータス

GA

## 概要

サードパーティコーディングエージェント（Claude、OpenAI Codex など）が生成するコードに対して、GitHub Copilot クラウドエージェントと同じ自動セキュリティ検証が適用されるようになった。CodeQL、GitHub Advisory Database、シークレットスキャンによる包括的なセキュリティチェックを提供。

## 詳細

サードパーティコーディングエージェントがリポジトリ内でコードを作成する際、GitHub が自動的にセキュリティ分析を実行する。

### セキュリティ検証プロセス

1. **CodeQL による脆弱性分析** — 生成されたコードの潜在的なセキュリティ脆弱性を検出
2. **依存関係チェック** — 新しく導入された依存関係を GitHub Advisory Database と照合
3. **シークレットスキャン** — API キーやトークンなどの機密情報を検出

### 自動修復

分析で問題が検出された場合、エージェントがプルリクエストを完了する前に問題の解決を試みる。

### 設定と利用条件

- デフォルトで有効（リポジトリの Copilot 設定に従う）
- Copilot クラウドエージェントのセキュリティ検証を既に有効にしている場合、サードパーティエージェントにも自動的に同じ保護が適用
- GitHub Advanced Security ライセンスは不要

### 背景

2025年10月に Copilot クラウドエージェント向けの自動コード検証をリリースして以来、数百件のセキュリティリークや脆弱性を事前に防止してきた実績がある。この保護をサードパーティエージェントにも拡張することで、どのコーディングエージェントが書いたコードであっても同じセキュリティチェックが適用される。

## 参考リンク

- [Security validation for third-party coding agents](https://github.blog/changelog/2026-06-09-security-validation-for-third-party-coding-agents/)
- [Risks and mitigations for GitHub Copilot cloud agent](https://docs.github.com/copilot/concepts/agents/cloud-agent/risks-and-mitigations#unvalidated-code-can-introduce-vulnerabilities)
- [エージェント設定の構成](https://docs.github.com/copilot/how-tos/use-copilot-agents/cloud-agent/configuring-agent-settings#enabling-or-disabling-built-in-code-quality-and-security-validation-tools)
