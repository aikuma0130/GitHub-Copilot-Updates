# Copilot オートメーションをコメントでトリガー可能に

## 日付

2026-08-03

## ステータス

GA

## 概要

Issue コメントや Pull Request コメントの作成をトリガーとして、Copilot Cloud Agent のオートメーションを実行できるようになった。ドキュメント生成、エラー調査、フォローアップタスク作成などのユースケースに対応。

## 詳細

オートメーション設定時にトリガーとなるコメントテキストを指定する。リポジトリの「Agents」タブから「Automations」を選択して設定可能。

主なユースケース:
- **ドキュメント生成**: PR にコメントしてコード変更に基づくドキュメントを自動生成・更新
- **エラー調査**: Issue にコメントしてスタックトレースやエラーログの調査を自動実行
- **フォローアップタスク作成**: PR にコメントしてリファクタリングや技術的負債の Issue を自動作成

Copilot Pro、Pro+、Max、Business、Enterprise ユーザーが利用可能。Business/Enterprise ユーザーは管理者による Copilot Cloud Agent ポリシーの有効化が必要。

## 参考リンク

- [Trigger Copilot automations with comments](https://github.blog/changelog/2026-08-03-trigger-copilot-automations-with-comments/)
- [About Copilot automations](https://docs.github.com/copilot/concepts/agents/cloud-agent/about-automations)
