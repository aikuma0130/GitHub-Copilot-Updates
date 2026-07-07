# C++ Language Server の設定スキルが Copilot CLI で利用可能に

## 日付

2026-07-01

## ステータス

GA

## 概要

Microsoft C++ Language Server が Copilot Plugins マーケットプレイスからインストール可能になり、プロジェクトセットアップを自動化する新しい設定スキルが追加されました。`compile_commands.json` の生成・管理がコマンド一つで行えるようになります。

## 詳細

### プラグインマーケットプレイスでの提供

C++ Language Server が Copilot CLI プラグインとして直接インストール可能になりました：

```
/plugin install cpp-language-server@copilot-plugins
```

以前の npm ベースのインストールに代わり、Windows、Linux、macOS でのセットアップとアップデートが簡素化されました。

### コンパイルコマンド生成スキル

新しい設定スキルにより、Copilot CLI から直接 `compile_commands.json` を生成・更新できます。「regenerate compile commands」または「load project」と入力するだけで、プロジェクトタイプとプラットフォームに基づいてコンパイルデータベースが自動構成されます。

Language Server は `compile_commands.json` の変更を自動監視するため、再起動なしで更新が反映されます。

### 対応プロジェクトタイプ

- **CMake**: スキルによる自動生成、または `-DCMAKE_EXPORT_COMPILE_COMMANDS=TRUE` オプションによるネイティブサポート
- **MSBuild**: スキルによるガイド付きセットアップ、またはサンプル抽出アプリケーションによる手動生成
- **カスタムビルドシステム**: プロジェクト固有のスキルを作成して繰り返し可能なセットアップを実現

### 4月のパブリックプレビューからの変更点

- npm パッケージからプラグインマーケットプレイスへの移行
- 組み込み設定スキルの追加（プロジェクトセットアップの自動化）
- クロスプラットフォームサポートの改善

## 参考リンク

- [New C++ language server config skill for Copilot CLI](https://github.blog/changelog/2026-07-01-new-c-language-server-config-skill-for-copilot-cli/)
- [Microsoft C++ Language Server リポジトリ](https://github.com/microsoft/cpp-language-server)
- [C++ Team ブログ: Streamline C++ Code Intelligence Setup in Copilot CLI](https://devblogs.microsoft.com/cppblog/streamline-c-code-intelligence-setup-in-copilot-cli/)
