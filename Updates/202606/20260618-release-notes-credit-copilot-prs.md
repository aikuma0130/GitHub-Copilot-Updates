# リリースノート自動生成で Copilot PR の貢献者がクレジットされるように

## 日付

2026-06-18

## ステータス

GA

## 概要

自動生成されるリリースノートで、Copilot クラウドエージェントが作成した PR について、指示を出した開発者が `@copilot` と並んでクレジットされるようになった。

## 詳細

GitHub のリリースノート自動生成機能で、Copilot クラウドエージェントが作成・マージした PR の表示形式が変更された。

### 変更前後の比較

- **変更前**: `Add create_feature_flag MCP tool by @copilot`
- **変更後**: `Add create_feature_flag MCP tool by @monalisa with @copilot`

これにより、Copilot クラウドエージェントを使って行った作業に対して、開発者が適切に認知される。エージェントが代わりに PR を作成した場合でも、指示を出した開発者の貢献が明確に示される。

### 利用可能範囲

すべてのリポジトリ、すべてのプランで利用可能。

## 参考リンク

- [Generated release notes credit you for Copilot pull requests](https://github.blog/changelog/2026-06-18-generated-release-notes-credit-you-for-copilot-pull-requests/)
