# Copilot CLI の Rubber Duck がより多くのモデルに対応

## 日付

2026-05-07

## ステータス

Improvement

## 概要

GitHub Copilot CLI のクロスファミリーレビューエージェント「Rubber Duck」が、GPT セッションでの Claude 批評エージェントの利用、および Claude セッションでの GPT-5.5 レビューアーモデルの利用をサポートし、セカンドオピニオン機能が強化されました。

## 詳細

### 新機能

- **GPT セッション向け Rubber Duck**: GPT モデルをオーケストレーターとして選択し `/experimental` を有効にしている場合、Claude ベースの Rubber Duck エージェントがセカンドオピニオンを提供。アーキテクチャ上の問題検出、微妙なバグの発見、ファイル間の競合検知が GPT セッションでも利用可能に
- **Claude セッション向けレビューアー強化**: Claude オーケストレーターのセッションで GPT-5.5 を Rubber Duck モデルとして利用可能になり、より効果的なセカンドオピニオンを実現

### 利用方法

1. `copilot` コマンドを実行
2. `/experimental on` を有効化
3. 通常通りコーディングを行うと、異なるモデルファミリーによるレビューが自動的に提供される

## 参考リンク

- [Rubber Duck in GitHub Copilot CLI now supports more models](https://github.blog/changelog/2026-05-07-rubber-duck-in-github-copilot-cli-now-supports-more-models)
- [GitHub Copilot CLI combines model families for a second opinion](https://github.blog/ai-and-ml/github-copilot/github-copilot-cli-combines-model-families-for-a-second-opinion/)
