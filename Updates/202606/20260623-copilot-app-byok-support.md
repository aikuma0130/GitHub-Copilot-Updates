# GitHub Copilot アプリが BYOK（Bring Your Own Key）に対応

## 日付

2026-06-23

## ステータス

GA

## 概要

GitHub Copilot アプリが BYOK に対応し、OpenAI、Azure OpenAI、Anthropic、LM Studio、Ollama など任意のモデルプロバイダーを使用してエージェントセッションを実行可能に。

## 詳細

### BYOK の概要

GitHub Copilot アプリの **Settings → Model Providers** からプロバイダーを追加し、エンドポイントと API キーを設定するだけで利用可能。LM Studio や Ollama の場合はホストの指定のみで接続できる。追加したプロバイダーのモデルは、Copilot ホステッドモデルと並んでモデルピッカーに表示される。

### 対応プロバイダー

- OpenAI
- Azure OpenAI
- Microsoft Foundry
- Anthropic
- LM Studio
- Ollama
- その他 OpenAI 互換エンドポイント

### 主なユースケース

- **既存プロバイダーとの接続**: 既存の課金、クォータ、リージョン、データ取扱い条件を維持したまま Copilot を利用
- **フロンティアモデルとローカルモデルの併用**: 複雑なタスクにはフロンティアモデル、実行にはローカルモデルを使い分け
- **テナント内でのトラフィック制御**: 自社クラウドアカウントや内部ゲートウェイ経由で推論をルーティングし、データ境界要件に対応

### セキュリティ

API キーはローカル OS のキーチェーンに保存され、UI からの読み戻しは行われない。

### 利用要件

Copilot Business / Enterprise プランのユーザーは、組織またはエンタープライズ管理者がポリシー設定で Copilot CLI を有効にする必要がある。

## 参考リンク

- [GitHub Copilot app support for BYOK](https://github.blog/changelog/2026-06-23-github-copilot-app-support-for-byok/)
- [Getting started with the GitHub Copilot app (docs)](https://docs.github.com/copilot/how-tos/github-copilot-app/getting-started)
- [Using your own LLM models in the Copilot app (docs)](https://docs.github.com/en/copilot/how-tos/github-copilot-app/use-byok-models)
- [GitHub Community Discussion](https://github.com/orgs/community/discussions/199307)
