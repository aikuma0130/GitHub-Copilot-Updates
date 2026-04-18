# Copilot CLI で自動モデル選択が一般提供開始

## 日付

2026-04-17

## ステータス

GA

## 概要

Copilot CLI で自動モデル選択（auto model selection）が全 Copilot プランで一般提供（GA）になりました。auto を選択すると、Copilot がユーザーのプランやポリシーに基づいて最適なモデルを自動的に選択します。

## 詳細

### 仕組み

auto モデル選択は動的にルーティングを行い、レート制限を緩和しつつ、GPT-5.4、GPT-5.3-Codex、Sonnet 4.6、Haiku 4.5 などのモデルに振り分けます。ルーティング対象のモデルは今後変更される可能性があります。

### 主な特徴

- **透明性**: Copilot CLI 上で実際に使用されたモデルを確認可能
- **制御の維持**: auto と特定モデルをいつでも切り替え可能
- **ポリシー準拠**: 管理者が設定したモデルポリシーを尊重

### プレミアムリクエストの課金

auto が選択するモデルは現在 0x〜1x の乗数を持つモデルに限定されています。有料サブスクライバーは auto 使用時にモデル乗数が 10% 割引されます（例: 1x 乗数のモデルの場合、1 ではなく 0.9 プレミアムリクエストとして計上）。

## 参考リンク

- [GitHub Copilot CLI now supports Copilot auto model selection](https://github.blog/changelog/2026-04-17-github-copilot-cli-now-supports-copilot-auto-model-selection/)
- [Copilot auto model selection ドキュメント](https://docs.github.com/copilot/concepts/auto-model-selection)
