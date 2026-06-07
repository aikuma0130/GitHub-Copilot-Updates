# Copilot CLI とエージェント機能の強化が JetBrains IDE で利用可能に

## 日付

2026-06-02

## ステータス

GA / Public Preview

## 概要

JetBrains IDE 向け GitHub Copilot に Copilot CLI セッション対応、エージェントピッカー、新スラッシュコマンド、エージェントデバッグパネル（プレビュー）、クラウドエージェント統合などを追加。

## 詳細

### Copilot CLI セッション関連

- **エージェントピッカー**: Agent モード（デフォルト）、Ask モード、カスタムエージェント、Plan モードを切り替え可能
- **新スラッシュコマンド**:
  - `/remote`: github.com や GitHub Mobile からセッションをリモートコントロール
  - `/compact`: セッションコンテキストを手動で圧縮
  - `/chronicle`: セッション履歴の分析とパーソナライズドティップスの取得
- **エージェントデバッグパネル**（パブリックプレビュー）: Copilot CLI セッション中のエージェントインタラクションの時系列イベントログを表示

### エージェント関連

- **クラウドエージェントの統合表示**: 統一セッションビューでクラウドエージェントセッションも表示
- **構成可能な思考努力レベル**: 対応モデルで推論の深さを調整可能
- **エージェントカスタマイズエディタ**: カスタムエージェントの設定を編集

### その他

- Google / Apple サインインオプションの追加
- Copilot CLI エージェントへのデフォルト体験の段階的移行開始

## 参考リンク

- [Introducing Copilot CLI and agentic capabilities enhancements in JetBrains IDEs](https://github.blog/changelog/2026-06-02-introducing-copilot-cli-and-agentic-capabilities-enhancements-in-jetbrains-ides/)
