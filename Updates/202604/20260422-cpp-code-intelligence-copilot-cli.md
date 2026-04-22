# C++ コードインテリジェンスが Copilot CLI でパブリックプレビュー

## 日付

2026-04-22

## ステータス

Public Preview

## 概要

Microsoft C++ Language Server が Copilot CLI のパブリックプレビューとして利用可能になりました。Visual Studio や VS Code と同じ IntelliSense エンジンを活用し、コマンドラインで精密なセマンティック C++ コードインテリジェンスを提供します。

## 詳細

### 背景

C++ は複雑な include 階層、マクロ、テンプレート、ビルドシステム依存の設定があるため、テキスト検索だけでは不完全な結果しか得られません。C++ Language Server は、シンボル定義、参照、コール階層、型情報などの精密なセマンティックデータを Copilot に提供し、grep スタイルの検索を補完します。

### 主な機能

- **シンボル検索と定義ジャンプ**: Copilot がワークスペースシンボル検索と go-to-definition を使用して、関連コードを直接検索・理解
- **マルチファイル編集**: 大規模な C++ コードベースでも複数ファイルにまたがるコード参照・更新を正確に実行
- **コンテキスト対応の提案**: シンボルの型、宣言、スコープ、使用法を考慮した、より正確で適切な提案

### 利用開始方法

Microsoft C++ Language Server は npm パッケージとして提供されています。利用には以下が必要です：

1. GitHub Copilot CLI での認証
2. プロジェクト用の `compile_commands.json` の作成
3. CLI で使用するためのプロジェクト設定

CMake プロジェクトでは、2番目と3番目の要件を自動処理するスキルが提供されています。MSBuild ユーザー向けには、`compile_commands.json` を抽出するサンプルアプリケーションが用意されています。

> **ヒント**: 最良の結果を得るには、クエリに「Use the C++ LSP」を追加するか、カスタムインストラクションファイルで C++ LSP の優先使用を設定してください。

## 参考リンク

- [C++ code intelligence for GitHub Copilot CLI in public preview](https://github.blog/changelog/2026-04-22-c-code-intelligence-for-github-copilot-cli-in-public-preview/)
- [Microsoft C++ Language Server リポジトリ](https://github.com/microsoft/cpp-language-server)
