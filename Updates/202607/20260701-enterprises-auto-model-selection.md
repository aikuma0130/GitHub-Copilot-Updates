# エンタープライズでオートモデル選択をデフォルト設定可能に

## 日付

2026-07-01

## ステータス

GA

## 概要

エンタープライズ管理者が `managed-settings.json` で「auto」をデフォルトのモデル選択モードに設定できるようになった。タスクに最適なモデルが自動的に選択され、品質・信頼性・コスト効率が向上する。

## 詳細

エンタープライズ管理者は `.github-private/.github/copilot/managed-settings.json` に `"model": "auto"` を追加することで、組織内の全ユーザーの新規会話でオートモデル選択をデフォルトにできる。

### 主な特徴

- タスクの複雑さ、システム状態、モデルパフォーマンスに基づき最適なモデルを自動選択
- ユーザーは個別の会話で手動でモデルを変更可能
- VS Code 1.126 以降、GitHub.com の Copilot Chat、Copilot CLI で利用可能
- Copilot Business および Copilot Enterprise プランで利用可能

### メリット

- ユーザーエクスペリエンスの簡素化
- 最新・最高パフォーマンスのモデルの自動利用
- コスト管理とガバナンスコンプライアンスの効率化

## 参考リンク

- [Enterprises can default to auto model selection](https://github.blog/changelog/2026-07-01-enterprises-can-default-to-auto-model-selection/)
- [About Copilot auto model selection - GitHub Docs](https://docs.github.com/en/copilot/concepts/models/auto-model-selection)
