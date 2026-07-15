# GitHub Copilot for JetBrains が BYOK 機能を拡張

## 日付

2026-07-14

## ステータス

GA / Public Preview（機能により異なる）

## 概要

JetBrains IDE 向け GitHub Copilot がカスタムエンドポイント対応、プラグイン管理の強化、Claude エージェントプロバイダーサポート、ローカルサンドボックスなど BYOK（Bring Your Own Key）機能を大幅に拡張した。

## 詳細

### カスタムエンドポイントサポート

OpenAI 互換のカスタムエンドポイントを自身の API キーで利用可能に。独自モデルや他プロバイダーへの接続が可能となり、企業の柔軟な運用を支援。

### プラグイン管理の強化

マーケットプレイスやソースリポジトリからプラグインを直接閲覧・インストール可能に。チームがワークフローに合わせて Copilot をカスタマイズできる。

### Claude エージェントプロバイダー

Copilot Pro 以上のプラン（パブリックプレビュー）で Claude エージェントプロバイダーを使用したカスタムエージェント・スキル・インストラクションの設定が可能に。

### ローカルサンドボックス

ローカルサンドボックスのサポートが追加され、JetBrains プラグイン内で新しいサンドボックス設定と構成が利用可能に（パブリックプレビュー）。

### Copilot CLI デバッガースキル

Copilot CLI に組み込みデバッガースキルが追加。会話型エージェントワークフローを通じたステップバイステップのデバッグが可能に（パブリックプレビュー）。

### UX 改善

- モデルピッカーの制御改善
- カスタムエージェント向け UI の明確化
- カスタマイズ可能な認証フロー
- メッセージの再編集によるプロンプト反復の高速化

### ポリシー変更

Copilot CLI をポリシーで無効化しても、JetBrains IDE 内の Copilot CLI プロバイダーは無効化されないよう変更。

## 参考リンク

- [GitHub Copilot for JetBrains expands BYOK capabilities](https://github.blog/changelog/2026-07-14-github-copilot-for-jetbrains-expands-byok-capabilities/)
