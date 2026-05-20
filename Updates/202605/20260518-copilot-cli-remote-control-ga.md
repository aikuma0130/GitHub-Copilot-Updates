# Copilot CLI セッションのリモートコントロールが GA（モバイル・Web・VS Code・JetBrains）

## 日付

2026-05-18

## ステータス

GA

## 概要

Copilot CLI セッションのリモートコントロール機能が正式リリース（GA）。ターミナルで開始したセッションを GitHub Mobile、github.com、VS Code、JetBrains からリアルタイムで監視・操作可能に。

## 詳細

### 変更内容

2026年4月13日のパブリックプレビューを経て、リモートコントロール機能が GA となった。開発者はターミナル、VS Code、JetBrains で Copilot CLI セッションを開始し、外出先からモバイルや Web でセッションを監視・操作できる。

### 新機能

- GitHub リポジトリに紐付かないディレクトリやリポジトリでも利用可能に
- VS Code および JetBrains からのリモートコントロール対応を新規追加

### モバイル・Web からできること

- セッション進捗のライブ追跡
- セッション途中での方向転換・メッセージのキュー追加
- 実装前のプラン確認・修正
- セッションの停止
- 権限リクエストの承認・拒否
- Copilot からの質問への応答

### Copilot CLI からの利用方法

- `copilot --remote` でリモートセッションを開始、または `/remote on` で途中から有効化
- QR コードのスキャンまたはリンクから GitHub Mobile / github.com で接続
- `/keep-alive` で長時間セッション中のマシンスリープ防止

### VS Code からの利用方法

- `github.copilot.chat.cli.remote.enabled` 設定を有効化
- Chat ビューから Copilot CLI セッションを開始
- `/remote on` でリモートコントロールを有効にし、GitHub タスクページを作成

### 管理者向け

Copilot Business / Enterprise ユーザーは、管理者がリモートコントロールおよび CLI ポリシーを有効にする必要がある。

## 参考リンク

- [Remote control for Copilot CLI sessions now generally available on mobile, web, and VS Code](https://github.blog/changelog/2026-05-18-remote-control-for-copilot-cli-sessions-now-generally-available-on-mobile-web-and-vs-code/)
- [Steer Copilot CLI sessions remotely](https://docs.github.com/en/copilot/how-tos/copilot-cli/steer-remotely)
- [About remote control](https://docs.github.com/en/copilot/concepts/agents/copilot-cli/about-remote-control)
