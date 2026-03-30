# Slack から Copilot で GitHub Issues を作成

## 日付

2026-03-30

## ステータス

GA

## 概要

Slack の GitHub アプリで `@GitHub` をメンションし、自然言語で GitHub Issues を直接作成できるようになりました。サブイシューの階層構造にも対応しています。

## 詳細

Slack 用 GitHub アプリに、Copilot を活用した Issue 作成機能が追加されました。チャンネル内で `@GitHub` をメンションし、自然言語で作業内容を記述するだけで、構造化された Issue がリポジトリに作成されます。

### 主な機能

- **自然言語での Issue 作成**: プレーンテキストで作業を記述すると、タイトル、本文、担当者、ラベル、マイルストーンを含む構造化された Issue が作成されます。
- **サブイシュー対応**: 1つのメッセージから親子関係を持つサブイシューを作成できます。
- **会話モード**: Slack スレッド内で `@GitHub` と対話しながら、Issue の詳細を作成前に調整できます。
- **Issue フレックスペイン**: 作成した Issue をタイトルクリックで Slack から直接確認できます。
- **チャンネルレベルの設定**: `@GitHub settings` コマンドで、チャンネルごとにデフォルトのリポジトリを設定できます。

### 利用条件

- すべての Copilot プラン（Free、Pro、Pro+、Business、Enterprise）で利用可能
- Slack ワークスペースに [GitHub アプリ](https://slack.com/marketplace/A01BP7R4KNY-github) のインストールまたはアップグレードが必要

## 参考リンク

- [Create issues from Slack with Copilot](https://github.blog/changelog/2026-03-30-create-issues-from-slack-with-copilot)
