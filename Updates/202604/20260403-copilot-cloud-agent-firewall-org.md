# Copilot cloud agent の Organization ファイアウォール設定

## 日付

2026-04-03

## ステータス

GA

## 概要

Organization 管理者が Copilot cloud agent のエージェントファイアウォールを Organization 全体で一元管理できるようになりました。ファイアウォールの有効/無効、推奨許可リスト、カスタム許可リストを Organization レベルで制御可能です。

## 詳細

Copilot cloud agent には、プロンプトインジェクションやデータ流出からの保護を目的としたエージェントファイアウォールが組み込まれています。従来はリポジトリレベルでの設定のみでしたが、Organization レベルでの管理が可能になりました。

### Organization 管理者が設定できる項目

- **ファイアウォールの有効/無効**: 全リポジトリ一括または各リポジトリ個別判断
- **推奨許可リストの有効/無効**: 全リポジトリ一括または各リポジトリ個別判断
- **Organization 全体のカスタム許可リスト**: 全リポジトリに適用されるエントリの追加（例: 内部パッケージレジストリへのアクセス許可）
- **リポジトリ管理者のカスタム許可リスト追加権限の制御**

### デフォルト動作

すべての設定はデフォルトで「各リポジトリに判断を委ねる」となっており、既存の動作が維持されます。

## 参考リンク

- [Organization firewall settings for Copilot cloud agent](https://github.blog/changelog/2026-04-03-organization-firewall-settings-for-copilot-cloud-agent)
- [Customizing the agent firewall for Copilot cloud agent](https://docs.github.com/copilot/how-tos/use-copilot-agents/coding-agent/customize-the-agent-firewall)
