# Copilot CLI の再設計されたターミナルインターフェースが一般提供開始

## 日付

2026-06-23

## ステータス

GA

## 概要

GitHub Copilot CLI の再設計されたターミナルインターフェースが一般提供開始。タブ付きレイアウト、ガイド付き設定、アクセシビリティ改善を含む新しい UI により、ターミナルから直接 GitHub と連携可能に。

## 詳細

### タブ付きレイアウトで Issue・PR・Gist をブラウズ

- セッション画面上部にタブが追加され、デフォルトの **Session** タブと **Gists** タブが利用可能
- GitHub リポジトリ内で実行すると **Issues** タブと **Pull requests** タブも表示
- ハイライトした Issue や PR に対して `c` キーでプロンプトに参照を挿入、`o` キーでブラウザで開く
- `/` キーで GitHub 検索クエリを実行可能
- マウスクリックでタブ切り替え、設定からタブの並べ替え・非表示・無効化が可能

### ターミナル内でのツール設定

手動での設定ファイル編集が不要に。

- **MCP サーバー**: `/mcp add` でインタラクティブフォーム、`/mcp search` で GitHub MCP Registry からサーバーを検索・インストール（再起動不要）
- **スキル**: `/skills` で矢印キーとスペースバーで個別に有効/無効を切り替え
- **プラグイン**: `/plugin` コマンドでマーケットプレイス、リポジトリ、ローカルパスからインストール
- **設定**: `/settings` ダイアログで設定をインラインで表示・変更

### アクセシビリティの改善

- テーマ対応のセマンティックカラーとレスポンシブコンポーネント
- `/theme` コマンドで `default`、`dim`、`high-contrast`、`colorblind` モードを選択可能
- スクリーンリーダー検出時に自動でサポートを有効化（ラベル付きアイコン、アニメーション無効化）

### アップデート方法

`copilot update` コマンドでアップデート可能。

## 参考リンク

- [Copilot CLI: New terminal interface is generally available](https://github.blog/changelog/2026-06-23-copilot-cli-new-terminal-interface-is-generally-available/)
- [Browsing issues, pull requests, and gists (docs)](https://docs.github.com/copilot/how-tos/copilot-cli/use-copilot-cli/browse-issues-prs-gists)
- [Customizing Copilot CLI (docs)](https://docs.github.com/copilot/how-tos/copilot-cli/customize-copilot/overview)
