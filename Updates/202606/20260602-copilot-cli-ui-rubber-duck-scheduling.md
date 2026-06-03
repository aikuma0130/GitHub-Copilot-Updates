# Copilot CLI: UI 改善、Rubber Duck、プロンプトスケジューリング、音声入力

## 日付

2026-06-02

## ステータス

GA / Experimental

## 概要

GitHub Copilot CLI に Rubber Duck、プロンプトスケジューリング、音声入力が GA で追加。実験的な新ターミナルインターフェース（タブ対応）もプレビュー提供開始。

## 詳細

### 新ターミナルエクスペリエンス（実験的）

`/experimental on` で有効化できるリデザインされたターミナルインターフェース：

- **タブ**: Session ビュー、Issues、Pull requests、Gists 間をタブで切り替え可能
- **テーマ対応カラー**: `default`、`github`、`dim`、`high-contrast`、`colorblind` などのカラーモード
- **アクセシビリティ**: スクリーンリーダー検出時に自動対応、ラベル付きアイコン、アニメーション自動無効化
- **一貫した UI コンポーネント**: ダイアログ、テーブル、リスト、見出しの統一的なレンダリング

### Rubber Duck（GA）

組み込みの CLI エージェントで、建設的な批評者として機能する：

- メインエージェントが計画、設計、実装、テストを Rubber Duck エージェントにレビュー依頼
- 盲点、設計の欠陥、実質的な問題を発見してフィードバック
- CLI が自動的に判断して第二の意見を求める場合がある
- `/rubber-duck` コマンドで手動呼び出しも可能

### プロンプトスケジューリング（GA）

新しい `/every` と `/after` スラッシュコマンド：

- **`/every`**: 指定間隔で繰り返しプロンプトを実行
  - 例: `/every 30m run the frontend tests`
  - 例: `/every 1h how many tokens have I used during the past hour`
- **`/after`**: 指定時間後に一度だけプロンプトを実行
  - 例: `/after 2h /example-skills:docx create a new file summarizing recent changes to this repo`
- 引数なしで実行するとスケジュールマネージャーを表示

### 音声入力（GA）

- スペースバー長押しで録音開始、離すと文字起こしが入力される
- または Ctrl+X → V で録音開始、任意のキーで停止
- 音声入力はローカルで処理され、音声データはマシン外に送信されない
- 初回使用時にランタイムのダウンロードと音声モデルの選択をガイド

## 参考リンク

- [Copilot CLI: Improved UI, rubber duck, prompt scheduling, and voice input](https://github.blog/changelog/2026-06-02-copilot-cli-improved-ui-rubber-duck-prompt-scheduling-and-voice-input/)
- [Rubber Duck ドキュメント](https://docs.github.com/copilot/concepts/agents/copilot-cli/rubber-duck)
- [Copilot CLI リポジトリ](https://github.com/github/copilot-cli)
