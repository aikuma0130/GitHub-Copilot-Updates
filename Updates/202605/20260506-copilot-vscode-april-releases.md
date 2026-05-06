# GitHub Copilot in Visual Studio Code — 4月リリースまとめ

## 日付

2026-05-06

## ステータス

GA

## 概要

VS Code の週次安定リリース（v1.116〜v1.119）における Copilot の主要アップデートをまとめたものです。セマンティック検索の全ワークスペース対応、BYOK のビジネス/エンタープライズ展開、エージェント機能の大幅強化、Copilot CLI セッションのリモート監視などが含まれます。

## 詳細

### スマートコンテキスト

- **全ワークスペースでのセマンティック検索**: セマンティックインデックスが全ワークスペースで動作するようになり、エージェントが `githubTextSearch` ツールで GitHub リポジトリや Organization に対して grep スタイルの検索も実行可能に
- **/chronicle（実験的機能）**: チャット履歴をローカルデータベースに記録し、過去のセッション検索や最近の作業の振り返りが可能。設定: `github.copilot.chat.localIndex.enabled`
- **トークン使用量の削減**: スマートプロンプトキャッシュ、遅延ツール読み込み、新しいエージェントツールによりリクエストごとのトークン使用量を削減

### エージェント体験

- **チャット内 diff 表示**: コード変更がチャットスレッド内に直接 diff として表示
- **エージェントカスタマイズの生成**: 自然言語の説明からカスタムエージェント、スキル、インストラクションのドラフトを作成
- **BYOK（Bring Your Own Key）**: Copilot Business/Enterprise ユーザーが独自の API キー（OpenRouter、Microsoft Foundry、Google、Anthropic、OpenAI 等）を接続可能。Ollama や Foundry Local でのローカルモデル実行もサポート
- **ターミナルアクセス**: エージェントが既存のフォアグラウンドターミナル（REPL やインタラクティブスクリプトを含む）の読み書きが可能に
- **統合ブラウザ**: タブ共有によりエージェントにライブブラウザへのアクセスを付与し、コンテンツの読み取り・ページ操作・リアルタイム検証が可能

### チャット継続性

- **Copilot CLI セッションのクロスデバイス継続（実験的）**: VS Code で開始した Copilot CLI セッションを GitHub.com やモバイルアプリからリモートで監視・操作可能。設定: `github.copilot.chat.cli.remote.enabled`
- **過去のエージェントセッションのデバッグ**: Agent Debug Log パネルがログをローカルに永続化し、過去のセッションの追跡が可能に
- **バックグラウンドコマンドの追跡**: 長時間実行されるターミナルコマンドがチャット内にシステム通知として表示

### その他

- **エージェントセッション UX の改善**: インクリメンタルチャットレンダリング、ソート可能なエージェントセッション、Copilot CLI との同期セッションタイトル
- **新しい Markdown プレビュー体験**: ツールバーボタンとコマンドで Markdown ソースとプレビューの切り替えが容易に

## 参考リンク

- [GitHub Copilot in Visual Studio Code, April releases](https://github.blog/changelog/2026-05-06-github-copilot-in-visual-studio-code-april-releases/)
- [VS Code Release Notes](https://aka.ms/VSCode/Release)
