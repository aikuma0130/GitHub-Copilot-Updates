# GitHub Desktop 3.6: ワークツリーと Copilot の深い統合

## 日付

2026-06-26

## ステータス

GA

## 概要

GitHub Desktop 3.6 がリリースされ、Copilot によるコミットメッセージ作成・マージコンフリクト解決の支援、および Git ワークツリーのネイティブサポートが追加された。

## 詳細

### Copilot SDK 基盤

GitHub Desktop の Copilot 機能は Copilot SDK 上に構築されており、すべての Copilot 機能でモデルピッカーによるモデル選択と BYOK（Bring Your Own Key）によるサードパーティ・ローカルモデル接続が可能。

### コミットメッセージ作成の強化

- `.github/copilot-instructions.md` や `AGENTS.md` のカスタムインストラクションを参照
- リポジトリのコミットメタデータルールに準拠したメッセージを自動生成
- リポジトリのスタイルや基準に合致したメッセージを生成

### Copilot によるコンフリクト解決

マージコンフリクト発生時に AI がコンフリクトの説明と解決案を提示。ユーザーはレビュー・編集後にマージを完了できる。

### Git ワークツリーサポート

- 複数ブランチでの並行作業が可能に
- ブランチ切り替えやスタッシュ、追加クローンが不要
- コーディングエージェントが分離・並列セッションで使用するワークツリーとの親和性が高い

### 対応プラットフォーム

macOS および Windows。Copilot 機能の利用には Copilot サブスクリプションが必要。

## 参考リンク

- [GitHub Desktop 3.6: Worktrees and deeper Copilot integration](https://github.blog/changelog/2026-06-26-github-desktop-3-6-worktrees-and-deeper-copilot-integration/)
- [GitHub Desktop releases](https://github.com/desktop/desktop/releases/tag/release-3.6.0)
