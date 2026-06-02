# 個人プランの Auto モデル選択で評価モデルが利用可能に

## 日付

2026-06-01

## ステータス

GA

## 概要

GitHub Copilot の個人（非エンタープライズ）ユーザー向けに、Auto モデル選択時に評価モデルが提供されるようになった。評価モデルの使用は設定から無効化可能。

## 詳細

### 変更内容

GitHub Copilot が個人（非エンタープライズ）ユーザーに対して評価モデル（Evaluation Models）へのアクセスを提供開始。Auto モデル選択が有効な場合、タスクの複雑さやシステムの状態に応じて評価モデルが自動的に選択される場合がある。

### Auto モデル選択の仕組み

Auto モデル選択は以下の要素を考慮してモデルを動的にルーティングする：

- タスクの複雑さ
- リアルタイムのシステムヘルス
- モデルの可用性
- コスト効率（シンプルなタスクには高速・低コストモデル、複雑なタスクにはより高性能なモデルを使用）

### 無効化方法

評価モデルの使用を望まない場合は、Copilot の設定から Auto モデル選択での評価モデル利用を無効化できる。

### 制約事項

- プランで利用不可のモデルは選択されない
- 管理者ポリシーでブロックされたモデルは選択されない
- コンプライアンスポリシーで制限されたモデルは選択されない

## 参考リンク

- [Evaluation models in auto for individual plans](https://github.blog/changelog/2026-06-01-evaluation-models-in-auto-for-individual-plans/)
- [About Copilot auto model selection](https://docs.github.com/en/copilot/concepts/models/auto-model-selection)
