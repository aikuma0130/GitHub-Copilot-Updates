# Copilot CLI のリモートセッション操作がパブリックプレビューで利用可能に

## 日付

2026-04-13

## ステータス

Public Preview

## 概要

Copilot CLI に `--remote` オプションが追加され、実行中の CLI セッションを Web や GitHub Mobile からリアルタイムで監視・操作できるようになりました。

## 詳細

Copilot CLI がローカル専用ツールから進化し、リモートセッション機能が追加されました。`copilot --remote` で起動すると、セッションの活動がリアルタイムで GitHub にストリーミングされます。

### 主な機能

- **リアルタイムストリーミング**: CLI セッションのアクティビティが GitHub にリアルタイムで配信
- **Web・モバイル対応**: リンクまたは QR コードを使って別のデバイスからセッションにアクセス可能
- **双方向同期**: CLI と GitHub 上の操作がリアルタイムで同期
- **セッションプライバシー**: 各リモートセッションは開始したユーザーのみが閲覧・操作可能

### サポートされる操作

- セッション中のステアリングメッセージの送信
- 実装計画のレビューと修正
- plan / interactive / autopilot モードの切り替え、セッション停止
- パーミッションリクエストの承認・拒否
- `ask_user` ツール経由の質問への応答

### 使い方

1. `/update` で Copilot CLI を最新バージョンに更新
2. `copilot --remote` で新しいリモートセッションを開始（既存セッションでは `/remote` コマンドで有効化）
3. 作業ディレクトリが GitHub リポジトリであることを確認
4. 表示されるリンクまたは QR コードから Web でセッションにアクセス
5. 長時間タスクでは `/keep-alive` でマシンのスリープを防止

### 利用条件

Copilot Business または Copilot Enterprise ユーザーの場合、管理者がリモートコントロールおよび CLI ポリシーを事前に有効化する必要があります。

## 参考リンク

- [Remote control CLI sessions on web and mobile in public preview](https://github.blog/changelog/2026-04-13-remote-control-cli-sessions-on-web-and-mobile-in-public-preview/)
- [Copilot CLI リモートアクセスについて](https://docs.github.com/en/copilot/concepts/agents/copilot-cli/about-remote-access)
- [Copilot CLI ドキュメント](https://docs.github.com/copilot/how-tos/copilot-cli/steer-remotely)
