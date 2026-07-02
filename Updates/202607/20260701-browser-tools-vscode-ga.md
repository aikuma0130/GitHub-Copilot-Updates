# VS Code の GitHub Copilot 用ブラウザツールが一般提供開始

## 日付

2026-07-01

## ステータス

GA

## 概要

VS Code のエージェントが実際のブラウザを操作し、ライブ Web アプリのナビゲーション・テスト・検証が可能に。デフォルトで有効化され、エンタープライズ管理機能も搭載。

## 詳細

### エージェントのブラウザ操作

エージェントが開発者と同等のブラウザアクションを実行可能：

- ページのオープン・ナビゲーション、クリック、入力、ホバー、ドラッグ、ダイアログ操作
- ページコンテンツの読み取り、コンソールエラーのキャプチャ、スクリーンショットの取得
- スクリプト化されたフローによる効率的な自動化

DevTools もブラウザツールバーに統合され、要素の検査やコンソール出力の確認が可能。

### プライバシーとセキュリティ

- **タブはデフォルトで非公開** — 「Share with Agent」を選択するまでエージェントはアクセス不可
- **エージェントのタブは分離** — エージェントが開いたページは独立セッションで動作し、通常ブラウジングの Cookie やストレージにアクセスしない
- **機密権限は承認が必要** — カメラ、マイク、位置情報、通知、クリップボード読み取りはエージェントが自動承認できず、明示的な許可が必要

### エンタープライズ管理

- 専用のオン/オフスイッチ（`workbench.browser.enableChatTools`）
- ネットワークドメイン制御（`chat.agent.allowedNetworkDomains` / `chat.agent.deniedNetworkDomains`）でアクセス可能サイトを制限
- ワイルドカード対応（例: `*.example.com`）、拒否リストが優先

## 参考リンク

- [Browser tools for GitHub Copilot in VS Code are generally available](https://github.blog/changelog/2026-07-01-browser-tools-for-github-copilot-in-vs-code-are-generally-available/)
