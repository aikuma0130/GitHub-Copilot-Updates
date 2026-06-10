# Claude Fable 5 が GitHub Copilot で一般提供開始

## 日付

2026-06-09

## ステータス

GA

## 概要

Anthropic の新しい Mythos クラスモデル「Claude Fable 5」が GitHub Copilot で一般提供開始。長期的な自律型コーディングおよびナレッジワークタスク向けに設計され、以前の Opus ティアモデルよりも少ないツールコールとトークン消費で同等の作業を完了。

## 詳細

Claude Fable 5 は Anthropic の Mythos クラスの最初のモデルで、長期的かつ自律的なコーディングタスクに最適化されている。

### 利用可能なプラン

- Copilot Pro+
- Copilot Max
- Copilot Business
- Copilot Enterprise

### 対応エディタ・ツール

- Visual Studio Code（Chat、Ask、Edit、Agent モード）
- Visual Studio
- Copilot CLI
- GitHub Copilot クラウドエージェント
- GitHub Copilot アプリ
- github.com
- GitHub Mobile（iOS / Android）
- JetBrains
- Xcode
- Eclipse

### データ保持に関する重要事項

- Claude Fable 5 は Anthropic の安全性分類器の運用のため、**データ保持が必要**
- プロンプトと出力が最大30日間保持される（有害・悪用検出目的）
- 30日後にデータは削除される
- 保持データはモデルのトレーニングには**使用されない**
- 他の Claude モデル（Opus 4.8、Sonnet 4.5、Haiku 4.5）は引き続きゼロデータ保持（ZDR）で動作

### 有効化方法

- Enterprise / Business プランの管理者が Copilot 設定で Claude Fable 5 ポリシーを明示的に有効化する必要がある
- デフォルトではオフ

### 課金

- Usage Based Billing のプロバイダーリスト価格で課金

## 参考リンク

- [Claude Fable 5 is generally available for GitHub Copilot](https://github.blog/changelog/2026-06-09-claude-fable-5-is-generally-available-for-github-copilot/)
- [GitHub Copilot で利用可能なモデル一覧](https://docs.github.com/copilot/reference/ai-models/supported-models)
- [Copilot の課金: モデルとリクエスト](https://docs.github.com/copilot/reference/copilot-billing/models-and-pricing)
- [Anthropic 商用利用規約・データ保持ポリシー](https://www.anthropic.com/legal/commercial-terms)
