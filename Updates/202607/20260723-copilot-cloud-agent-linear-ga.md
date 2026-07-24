# Copilot クラウドエージェントの Linear 連携が GA

## 日付

2026-07-23

## ステータス

GA

## 概要

Copilot クラウドエージェントの Linear 連携が一般提供開始。Linear 上の Issue を Copilot クラウドエージェントに割り当てることで、自律的にコードを分析しドラフト PR を作成可能に。

## 詳細

### 主な機能

- **Issue の自動対応**: Linear 上の Issue を Copilot クラウドエージェントにアサインすると、エージェントが Issue の内容を分析し、対応するコード変更を行いドラフト PR を作成
- **コンテキストの自動引き継ぎ**: Linear の Issue に記載された要件、仕様、関連情報が自動的にエージェントに渡される
- **進捗の自動更新**: エージェントの作業進捗が Linear 上でリアルタイムに反映される
- **GitHub リポジトリとのシームレスな連携**: PR 作成、レビュー依頼、マージまでのワークフローを自動化

### 利用要件

- GitHub の組織オーナー権限
- Linear のワークスペース管理者権限
- Copilot Business または Enterprise プラン

### 背景

2025年10月にパブリックプレビューとして提供開始された本機能が、正式に一般提供（GA）となった。

## 参考リンク

- [Copilot cloud agent for Linear is generally available](https://github.blog/changelog/2026-07-23-copilot-cloud-agent-for-linear-is-generally-available/)
- [GitHub Copilot for Linear available in public preview](https://github.blog/changelog/2025-10-28-github-copilot-for-linear-available-in-public-preview/)
- [Integrating Copilot cloud agent with Linear - GitHub Docs](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/cloud-agent/integrate-cloud-agent-with-linear)
