# GitHub Copilot in Eclipse: BYOK、スキル、チャット更新

## 日付

2026-06-02

## ステータス

GA

## 概要

Eclipse 向け Copilot プラグインが大幅アップデート。BYOK（Bring Your Own Key）、スキル/プロンプトファイル対応、チャット UI 刷新、ABAP サポート強化、推論ブロック表示などを追加。

## 詳細

### チャット UI の刷新

- 新しいコンボピッカーでチャットモードとモデルを選択
- コンテキストウィンドウ使用量をドーナツインジケーターで表示
- セッションごとのトークン使用量の内訳を確認可能

### BYOK（Bring Your Own Key）

- Copilot Business / Enterprise ユーザーが BYOK を利用可能に
- 組織管理者が有効化後、サポート対象プロバイダーの API キーを設定してカスタムモデルを利用可能

### スキルとプロンプトファイル

- `/.github/skills/` 配下にスキルファイルを定義
- `/.github/prompts/` 配下にプロンプトファイルを定義
- チャット入力で `/` を入力してスラッシュコマンドピッカーから呼び出し可能

### その他の改善

- ABAP 開発のサポート向上
- カスタムインストラクションの読み込み設定（全プロジェクト / 参照プロジェクトのみ）
- 思考ブロックの表示対応
- 思考努力レベルの選択機能

## 参考リンク

- [GitHub Copilot in Eclipse: BYOK, skills, and chat updates](https://github.blog/changelog/2026-06-02-github-copilot-in-eclipse-byok-skills-and-chat-updates/)
