# Copilot CLI のオートモデル選択がタスクに基づいてルーティング

## 日付

2026-07-01

## ステータス

GA

## 概要

Copilot CLI のオートモデル選択が、リアルタイムのモデル可用性・信頼性シグナルとタスクの特性を評価し、最適なモデルに自動ルーティングするようになった。有料プランでは AI クレジットが 10% 割引される。

## 詳細

### 仕組み

Auto は以下の観点でタスクを評価し、最適なモデルを選択する：

- 推論の複雑さ
- コード生成の難易度
- バグ診断の困難さ
- ツールオーケストレーションの必要性

リアルタイムのモデル可用性と信頼性シグナルも考慮される。

### 主な特徴

- `/model` コマンドでいつでも Auto と特定モデルを切り替え可能
- 管理者が設定したモデルポリシーを尊重
- 複数のモデルファミリーを活用（サブスクリプションとポリシーに依存）

### AI クレジット

- Auto が選択したモデルのレートに基づいて課金
- 有料サブスクライバーは Auto 使用時に 10% 割引（同じモデルを直接使用する場合より 10% 少ない AI クレジット消費）
- レガシー年間プラン利用者はプレミアムリクエストベースの課金が継続

### トークン効率

Auto は自然なキャッシュ境界に沿ってルーティングするため、不要なキャッシュ関連コストを回避。品質を維持しながらトークン効率が向上する。

## 参考リンク

- [Copilot CLI auto model selection routes based on task](https://github.blog/changelog/2026-07-01-copilot-cli-auto-model-selection-routes-based-on-task/)
- [About auto model selection - GitHub Docs](https://docs.github.com/copilot/concepts/auto-model-selection)
