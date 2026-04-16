# GitHub CLI でエージェントスキルの管理が可能に

## 日付

2026-04-16

## ステータス

Public Preview

## 概要

GitHub CLI に新コマンド `gh skill` が追加され、AI コーディングエージェント向けのスキルの検索・インストール・管理・公開がコマンドラインから可能になりました。

## 詳細

### エージェントスキルとは

エージェントスキルは、AI エージェントに特定のタスクの実行方法を教えるための、ポータブルな命令・スクリプト・リソースのセットです。オープンな [Agent Skills 仕様](https://agentskills.io) に準拠しており、GitHub Copilot、Claude Code、Cursor、Codex、Gemini CLI など複数のエージェントホストで動作します。

### 基本的な使い方

GitHub CLI v2.90.0 以降にアップデートして利用できます。

```bash
# リポジトリのスキルを対話的にインストール
gh skill install github/awesome-copilot

# 特定のスキルを直接インストール
gh skill install github/awesome-copilot documentation-writer

# タグ指定でバージョンを固定してインストール
gh skill install github/awesome-copilot documentation-writer@v1.2.0

# スキルの検索
gh skill search mcp-apps
```

### バージョン固定とサプライチェーンセキュリティ

パッケージマネージャーと同等のセキュリティ保証を提供します：

- **タグとリリース**: `gh skill publish` で不変リリースの有効化を提案
- **コンテンツアドレスベースの変更検出**: git ツリー SHA を記録し、実際のコンテンツ変更を検出
- **バージョン固定**: `--pin` オプションでタグやコミット SHA にロック
- **ポータブルな来歴情報**: インストール時にメタデータを `SKILL.md` のフロントマターに記録

### スキルの公開

```bash
# すべてのスキルを検証
gh skill publish

# メタデータの問題を自動修正
gh skill publish --fix
```

### 対応エージェントホスト

| ホスト | コマンド例 |
|--------|-----------|
| GitHub Copilot | `gh skill install OWNER/REPO SKILL` |
| Claude Code | `gh skill install OWNER/REPO SKILL --agent claude-code` |
| Cursor | `gh skill install OWNER/REPO SKILL --agent cursor` |
| Codex | `gh skill install OWNER/REPO SKILL --agent codex` |
| Gemini CLI | `gh skill install OWNER/REPO SKILL --agent gemini` |
| Antigravity | `gh skill install OWNER/REPO SKILL --agent antigravity` |

### 注意事項

スキルはユーザーの判断でインストールされます。GitHub による検証は行われておらず、プロンプトインジェクション、隠された命令、悪意のあるスクリプトが含まれる可能性があります。インストール前に `gh skill preview` コマンドでコンテンツを確認することが推奨されます。

## 参考リンク

- [Manage agent skills with GitHub CLI](https://github.blog/changelog/2026-04-16-manage-agent-skills-with-github-cli)
- [Agent Skills 仕様](https://agentskills.io)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions)
