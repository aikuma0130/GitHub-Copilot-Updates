# GitHub Copilot in Visual Studio — 3月アップデート

## 日付

2026-04-02

## ステータス

GA

## 概要

Visual Studio 2026 の3月アップデートで、Copilot の拡張性が大幅に強化されました。カスタムエージェント、エージェントスキル、シンボル検索ツールなど、エージェントをよりスマートで高機能にする新機能が追加されています。

## 詳細

### 主なハイライト

- **カスタムエージェントの構築**: リポジトリ内の `.agent.md` ファイルで専用 Copilot エージェントを定義可能。ワークスペース認識、コード理解、ツール、好みのモデル、MCP 接続へのフルアクセスが可能
- **Enterprise MCP ガバナンス**: MCP サーバーの使用が GitHub で設定された許可リストポリシーに準拠。管理者が Organization 内で許可される MCP サーバーを指定可能
- **エージェントスキル**: 再利用可能な指示セットでエージェントに特定タスクの実行方法を学習させる。リポジトリやユーザープロファイルに定義し、Copilot が自動的に発見・適用
- **`find_symbol` ツール**: エージェントモードに言語対応のシンボルナビゲーションを追加。参照検索、型メタデータアクセス、宣言とスコープの理解をサポート（C++、C#、Razor、TypeScript 等）
- **Copilot によるテストプロファイリング**: Test Explorer の新しい「Profile with Copilot」コマンドで、テストを自動実行し CPU・インストルメンテーションデータを分析
- **ライブプロファイリングによる PerfTips**: デバッグ中のパフォーマンスシグナルを Profiler Agent と連携し、経過時間・CPU 使用率・メモリ動作を分析して最適化を提案
- **スマート Watch 候補**: デバッグ中の Watch ウィンドウでコンテキストに応じた式の候補を直接提示
- **Copilot で脆弱性を修正**: NuGet パッケージの脆弱性を Solution Explorer から直接修正。「Fix with GitHub Copilot」リンクでターゲットの依存関係更新を推奨

## 参考リンク

- [GitHub Copilot in Visual Studio — March update](https://github.blog/changelog/2026-04-02-github-copilot-in-visual-studio-march-update)
- [Visual Studio Blog](https://devblogs.microsoft.com/visualstudio/visual-studio-march-update-build-your-own-custom-agents/)
- [Visual Studio 2026 リリースノート](https://learn.microsoft.com/visualstudio/releases/2026/release-notes)
