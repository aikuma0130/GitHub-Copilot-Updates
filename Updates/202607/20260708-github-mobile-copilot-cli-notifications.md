# GitHub Mobile で Copilot CLI セッションのライブ通知が利用可能に

## 日付

2026-07-08

## ステータス

GA

## 概要

GitHub Mobile がリモート Copilot CLI セッションのリアルタイム通知に対応。進捗確認、入力待ち通知、セッション再開がモバイルから可能に。

## 詳細

リモートで実行中の Copilot CLI セッションについて、GitHub Mobile がリアルタイムの更新を表示できるようになった。iOS のライブアクティビティと Android のライブ更新通知を活用し、セッションの状態を確認してタップでセッションログビューに移動できる。

### 対応するセッション状態

- 進行中（In progress）
- ユーザー入力待ち（Waiting for user input）
- アイドル（Idle）
- 完了（Finished）

### 対象プラットフォーム

Copilot CLI、VS Code、その他のサポートされたサーフェスから起動されたリモートセッションを監視可能。

### 要件

- iOS: ライブアクティビティには iOS 17.2 以降が必要
- Android: ライブ更新通知には Android 16 以降が必要（古いバージョンでも通常のプログレス通知は受信可能）

### 無効化

設定から無効化が可能。最初のライブ通知にも「Disable Live Updates」ボタンが含まれる。

## 参考リンク

- [GitHub Mobile: Live notifications for Copilot CLI sessions](https://github.blog/changelog/2026-07-08-github-mobile-live-notifications-for-copilot-cli-sessions/)
