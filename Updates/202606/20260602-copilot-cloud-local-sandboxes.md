# GitHub Copilot のクラウド・ローカルサンドボックスがパブリックプレビュー

## 日付

2026-06-02

## ステータス

Public Preview

## 概要

GitHub Copilot がセキュアで分離されたサンドボックス（ローカルおよびクラウド）で実行可能に。エージェントワークフローの安全性と制御性を確保する。

## 詳細

### 背景

Copilot がツール実行、コマンド実行、ファイル変更を行うエージェントに進化する中、開発者や企業にはセキュリティ、分離、制御に関するより強固な保証が必要になっている。

### ローカルサンドボックス

- `/sandbox enable` でセッション内のサンドボックスを有効化
- Copilot が実行するシェルコマンドのファイルシステム、ネットワーク、システム機能へのアクセスを制限
- Microsoft MXC テクノロジーに基づき、macOS / Linux / Windows で一貫した分離エクスペリエンスを提供
- 企業は Microsoft Intune やその他の MDM プラットフォームでサンドボックスポリシーを一元管理可能
- 標準の GitHub Copilot シートに含まれる

### クラウドサンドボックス

- `copilot --cloud` で完全に分離されたエフェメラル Linux サンドボックスを起動
- 既存の Copilot クラウドエージェントポリシーを継承
- デバイス間でセッションを継続可能
- コンピュートインテンシブなワークフローのオフロードと並列実行が可能

### 主なユースケース

- エージェント実行に対するより強力なセキュリティ境界
- Copilot のツール実行の分離によるマシンの保護
- macOS / Linux / Windows での標準化された分離エクスペリエンス
- エンタープライズ向けの一元的なサンドボックスポリシー管理

## 参考リンク

- [Cloud and local sandboxes for GitHub Copilot now in public preview](https://github.blog/changelog/2026-06-02-cloud-and-local-sandboxes-for-github-copilot-now-in-public-preview/)
- [サンドボックスドキュメント](https://docs.github.com/copilot/concepts/about-cloud-and-local-sandboxes)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/197220)
