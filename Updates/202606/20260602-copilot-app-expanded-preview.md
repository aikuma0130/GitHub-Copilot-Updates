# GitHub Copilot アプリのテクニカルプレビューが拡大

## 日付

2026-06-02

## ステータス

Technical Preview

## 概要

GitHub Copilot アプリのテクニカルプレビューが全 Copilot Pro / Pro+ / Business / Enterprise ユーザーに拡大。新機能「キャンバス」により、エージェントと人間の協調作業が可能に。

## 詳細

### 利用可能なユーザー

- Copilot Pro、Pro+、Business、Enterprise の既存ユーザーは即時利用可能
- Copilot Free ユーザーはウェイトリストに参加可能
- Pro+ ユーザーは Copilot Max へのアップグレードが可能

### 新機能：キャンバス（Canvases）

キャンバスは人間とエージェントの双方向作業サーフェスで、エージェント作業を可視化・検証するための新しいインターフェース。

3つの参加者がキャンバスを共有する：

- **ユーザー**: 状態の検査、方向の修正、編集、進捗の検証
- **エージェント**: キャンバス状態の読み取り、構造化されたアクション、サーフェスの更新、完了のエビデンスとして使用
- **アプリ**: キャンバスを基になるアーティファクトやランタイムに接続し、許可されるアクションを制御

### その他の新機能

- **音声会話**: オンデバイス音声テキスト変換によるハンズフリー入力（音声データはローカルに留まる）
- **クラウドセッション**: アプリ UI からクラウドでエージェントセッションを実行
- **クラウドオートメーション**: 定期的なタスクをクラウドでスケジュール実行
- **Copilot CLI セッションの統合**: CLI で開始したセッションが My work ビューに表示
- **エージェントブラウジング**: 統合ブラウザをエージェントが操作（クリック、入力、スクリーンショット）して UI 変更をエンドツーエンドで検証
- **Rubber duck**: 問題をコミット前に話し合うための組み込みスキル
- **`/chronicle`**: 外部で開始したセッションを含む、すべてのエージェントセッションのデータをクエリ

### Copilot アプリの主な機能

- イシュー、PR、プロンプト、過去のセッションからセッションを開始
- 並列エージェントセッション（各セッションは独自の git worktree とブランチ）
- git リポジトリ以外のローカルフォルダからも開始可能
- 統合ターミナルとブラウザでの検証
- Agent Merge によるレビューコメント対応、失敗チェックの修正、マージ

## 参考リンク

- [Expanded technical preview availability for the GitHub Copilot app](https://github.blog/changelog/2026-06-02-expanded-technical-preview-availability-for-the-github-copilot-app/)
- [Copilot アプリのダウンロード](https://github.com/github/app)
- [Copilot アプリのドキュメント](https://docs.github.com/copilot/how-tos/github-copilot-app/getting-started)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/197303)
