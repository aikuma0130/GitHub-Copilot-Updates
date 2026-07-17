# Copilot Code Review のカスタマイズと設定機能の改善

## 日付

2026-07-17

## ステータス

GA

## 概要

Copilot Code Review がファイアウォール、カスタムセットアップステップ、独立したランナー設定に対応。head ブランチからカスタム指示を読み取り可能になり、レビューワークフローの柔軟性が向上。

## 詳細

### 新機能

- **ファイアウォール対応**: Code Review プロセスのセキュリティを強化
- **カスタムセットアップステップ**: レビュー環境のセットアップをカスタマイズ可能に
- **独立したランナー設定**: Code Review 用に専用のランナーを設定可能

### head ブランチからのカスタム指示読み取り

従来はベースブランチ（main 等）のカスタム指示ファイルのみが使用されていたが、本アップデートにより head ブランチ（PR のソースブランチ）からもカスタム指示を読み取り可能に。

これにより以下が可能になった：
- カスタム指示の変更をマージ前にテスト・検証
- ブランチごとに異なるレビュー設定を試行
- レビューワークフローの段階的なロールアウト

### カスタム指示のベストプラクティス

- 指示は簡潔かつ具体的に記述
- `.github/copilot-instructions.md` でリポジトリ全体またはパス固有の設定を管理

## 参考リンク

- [Copilot code review: Customization and configurability improvements](https://github.blog/changelog/2026-07-17-copilot-code-review-customization-and-configurability-improvements/)
- [Using custom instructions to unlock the power of Copilot code review](https://docs.github.com/en/copilot/tutorials/customize-code-review)
