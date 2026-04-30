# GitHub Copilot in Visual Studio — 4月アップデート

## 日付

2026-04-30

## ステータス

GA

## 概要

Visual Studio 2026 の4月アップデートでエージェントワークフローが大幅に強化され、IDE からの cloud agent セッション起動、ユーザーレベルのカスタムエージェント、新しいデバッガーエージェントによるランタイム検証が追加されました。

## 詳細

### Cloud agent 統合

Visual Studio から直接 cloud agent セッションを開始可能に。エージェントピッカーで「Cloud」を選択してタスクを記述すると、cloud agent がリモートインフラ上で GitHub Issue とプルリクエストを作成します。ローカルでの作業を中断せずにタスクを委任できます。

### ユーザーレベルのカスタムエージェント

カスタムエージェントがユーザーレベルの定義に対応。`%USERPROFILE%/.github/agents/` に保存したエージェント定義がプロジェクトをまたいで利用可能になり、個人のエージェントをどのプロジェクトでも使えるようになりました。

### エージェントスキルの拡張

エージェントスキルの検出パスが拡張され、既存の `.github/skills/` に加えて `.claude/skills/` や `.agents/skills/` ディレクトリからも検出されるようになりました。チームのワークフローに合った規約でスキルを整理できます。

### デバッガーエージェント

新しいデバッガーエージェントワークフローにより、ライブ実行に対するバグ検証が可能に。GitHub や Azure DevOps の Issue から開始し、エージェントが再現・計測・診断・修正提案をライブ実行を通じて行います。

### その他の改善

- **カスタマイズ可能なキーボードショートカット**: Copilot インライン提案の承認キーをカスタマイズ可能に（`Edit.AcceptSuggestion`、`Edit.AcceptNextWordInSuggestion`、`Edit.AcceptNextLineInSuggestion`）
- **新しいチャット履歴パネル**: チャットセッションのタイトル、メッセージプレビュー、タイムスタンプを表示する専用の履歴パネルを追加
- **C++ コード編集ツールの GA**: エージェントモード向け C++ コード編集ツール（`get_symbol_call_hierarchy`、`get_symbol_class_hierarchy`）が一般提供開始
- **テキストビジュアライザーの自動デコード**: テキストビジュアライザーに「Auto-detect and format」ボタンを追加。Copilot がエンコーディングや圧縮形式を識別して自動デコードします

## 参考リンク

- [GitHub Copilot in Visual Studio — April update](https://github.blog/changelog/2026-04-30-github-copilot-in-visual-studio-april-update/)
- [Visual Studio ブログ](https://devblogs.microsoft.com/visualstudio/visual-studio-april-update-cloud-agent-integration)
- [Visual Studio 2026 リリースノート](https://learn.microsoft.com/visualstudio/releases/2026/release-notes)
- [Visual Studio ダウンロード](https://visualstudio.microsoft.com/downloads)
