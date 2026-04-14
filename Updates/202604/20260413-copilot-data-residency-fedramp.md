# Copilot データレジデンシー（US + EU）と FedRAMP コンプライアンスが利用可能に

## 日付

2026-04-13

## ステータス

GA

## 概要

GitHub Copilot が米国および EU リージョンのデータレジデンシーをサポートし、推論処理と関連データが指定地域内に留まるようになりました。米国政府顧客向けに FedRAMP Moderate 認定にも対応しています。

## 詳細

GitHub Copilot がデータレジデンシーと FedRAMP コンプライアンスに対応しました。

### 対象機能

すべての GA 済み Copilot 機能がサポートされます：エージェントモード、インライン提案、チャット、Copilot cloud agent、コードレビュー、プルリクエスト要約、Copilot CLI。すべての機能が指定リージョン内のコンプライアンス認定済みモデルエンドポイントを使用します。

### モデル可用性

OpenAI と Anthropic の幅広いモデルが利用可能です（GPT-5.4、Claude Sonnet 4.6、Claude Opus 4.6 など）。Gemini モデルは GCP がデータレジデント推論エンドポイントを提供していないため、現時点では未サポートです。

### 料金

データレジデンシーおよび FedRAMP リクエストには、モデル乗数が **10% 増加** します。例えば、通常1プレミアムリクエストのモデルは、データレジデンシー下で1.1プレミアムリクエストになります。

### 利用開始方法

Enterprise および Organization の管理者が Copilot 設定からデータレジデンシーおよび FedRAMP ポリシーを有効にできます。ポリシーはデフォルトでオフのため、明示的なオプトインが必要です。

現在は US および EU リージョンがサポートされており、日本やオーストラリアなどの追加リージョンは 2026 年後半に対応予定です。

## 参考リンク

- [Copilot data residency in US + EU and FedRAMP compliance now available](https://github.blog/changelog/2026-04-13-copilot-data-residency-in-us-eu-and-fedramp-compliance-now-available)
- [データレジデンシーに関するドキュメント](https://docs.github.com/enterprise-cloud@latest/admin/data-residency/github-copilot-with-data-residency)
- [FedRAMP モデルに関するドキュメント](https://docs.github.com/copilot/concepts/fedramp-models)
