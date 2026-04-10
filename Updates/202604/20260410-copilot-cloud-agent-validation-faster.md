# Copilot cloud agent のバリデーションツールが 20% 高速化

## 日付

2026-04-10

## ステータス

GA

## 概要

Copilot cloud agent のセキュリティ・品質バリデーションツール（CodeQL、GitHub Advisory Database、シークレットスキャン、Copilot コードレビュー）が並列実行に変更され、バリデーション時間が 20% 短縮されました。

## 詳細

Copilot cloud agent がコードを記述する際、GitHub のセキュリティおよび品質バリデーションツールが自動的に実行されます。これまで順次実行されていたこれらのツールが並列実行に変更され、品質を維持しながらバリデーション時間が 20% 短縮されました。

### バリデーションツール

- [CodeQL](https://docs.github.com/code-security/code-scanning/introduction-to-code-scanning/about-code-scanning-with-codeql)
- [GitHub Advisory Database](https://docs.github.com/code-security/security-advisories/working-with-global-security-advisories-from-the-github-advisory-database)
- [シークレットスキャン](https://docs.github.com/code-security/secret-scanning/introduction/about-secret-scanning)
- [Copilot コードレビュー](https://docs.github.com/copilot/using-github-copilot/code-review/using-copilot-code-review)

### 設定

cloud agent が実行するバリデーションツールは、リポジトリ設定の **Copilot → Cloud agent** セクションから設定可能です。

## 参考リンク

- [Copilot cloud agent's validation tools are now 20% faster](https://github.blog/changelog/2026-04-10-copilot-cloud-agents-validation-tools-are-now-20-faster)
- [Copilot cloud agent ドキュメント](https://docs.github.com/copilot/concepts/agents/cloud-agent/about-cloud-agent)
