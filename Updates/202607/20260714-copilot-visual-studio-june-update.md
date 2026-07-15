# GitHub Copilot in Visual Studio — 2026年6月アップデート

## 日付

2026-07-14

## ステータス

GA

## 概要

Visual Studio 2026 の Copilot に使用量トラッキング・課金アラート、MCP サーバーの信頼性検証、C++ モダナイゼーションエージェントの GA、長距離次編集提案、PR レビュー統合などが追加された。

## 詳細

### 使用量トラッキングとアラート

リニューアルされた **Copilot Usage** ウィンドウが使用量ベースの課金モデルに対応し、リアルタイムで更新される。使用量が上限に近づいた時、到達した時、超過が発生した時にプロアクティブなアラートが通知される。警告閾値は設定でカスタマイズ可能。

### MCP サーバーの信頼性検証

Visual Studio が起動時に MCP サーバーの設定とアセットフィンガープリントを信頼済みベースラインと比較する。変更が検出された場合、サーバー実行前に信頼ダイアログで確認が求められる。デフォルトで有効。

### C++ モダナイゼーションエージェントが GA

MSVC アップグレードシナリオ向けのモダナイゼーションエージェントがプレビューを卒業。**Automated** モードでエンドツーエンドのアップグレード、**Guided** モードでステップごとのレビューが可能。

### 長距離次編集提案

Copilot の次編集提案がカーソル近辺だけでなく、アクティブファイル内のどこでもフォローアップ編集を予測・提案できるようになった。

### PR を Copilot Chat に追加

Git Repository ウィンドウで PR を右クリックし「Add to Copilot Chat」を選択すると、PR の説明・変更ファイル・コメントがコンテキストとして利用可能に。`#` + PR ID でインライン参照も可能。

### IDE 内 PR レビュー

GitHub または Azure DevOps の PR を IDE 内で閲覧・コメント・承認・完了可能に。Copilot Chat と連携してトリアージやサマリー作成を支援。

## 参考リンク

- [GitHub Copilot in Visual Studio — June update](https://github.blog/changelog/2026-07-14-github-copilot-in-visual-studio-june-update/)
- [Visual Studio blog](https://devblogs.microsoft.com/visualstudio/visual-studio-june-update-track-your-usage-trust-your-tools)
