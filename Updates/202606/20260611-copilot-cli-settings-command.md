# Copilot CLI: /settings でまとめて設定可能に

## 日付

2026-06-11

## ステータス

GA

## 概要

Copilot CLI に新しい `/settings` コマンドが追加され、すべてのユーザー設定をインタラクティブなダイアログから一元的にブラウズ・編集可能に。JSON ファイルの手動編集が不要になり、設定管理が大幅に簡素化。

## 詳細

### /settings コマンド

`/settings` と入力すると、ターミナル内でグラフィカルな設定ブラウザ/エディタが起動する。エージェント、ツール、UI レイアウトなど、すべての設定項目を対話的に閲覧・変更可能。変更は即時保存される。

### その他の改善点

- **UI の改善**: `/agents` ピッカーと「Create New Agent」ウィザードのボーダー・ヘッダー・入力欄を視覚的に統一
- **バグ修正**: メモリ無効時のセッション再開で空白画面になる問題を修正
- **コマンド発見性**: `/after` と `/every` が `/experimental` に表示されるように
- **ホームタブ設定**: タブバーの表示・順序・非表示タブを `settings.json` の `tabs` で設定可能に
- **ピッカー改善**: `/agent` 等のピッカーで数字キー選択が10番目以降にも拡張
- **シンボリックリンク**: `@-file` ピッカーでシンボリックリンクされたディレクトリが候補に表示
- **セッション管理**: `/sessions` がセッションタブに直接遷移
- **mTLS サポート**: OTLP テレメトリエクスポートで mTLS とプライベート CA をサポート
- **フルスクリーンスクロールバー**: 新規追加
- **ライトテーマ**: アクセシビリティ向上のための改善

## 参考リンク

- [Copilot CLI: Configure everything from one place with /settings](https://github.blog/changelog/2026-06-11-copilot-cli-configure-everything-from-one-place-with-settings/)
