# Copilot CLI/SDK で AI クレジットセッション制限が設定可能に

## 日付

2026-07-01

## ステータス

Public Preview

## 概要

Copilot CLI および GitHub Copilot SDK でセッションごとの AI クレジット使用上限を設定可能に。自動化ジョブでの予期しないコスト超過を防止する機能。

## 詳細

### 機能概要

セッション開始前またはジョブ実行前に制限を設定すると、Copilot がモデル呼び出し・サブエージェント・バックグラウンド作業を含むセッション全体の AI クレジット使用量を追跡。制限に達するとエージェントが処理を終了して通知する。

### 使用方法

- **対話型セッション**: `/limits` コマンドで制限の表示・設定・解除が可能。制限到達時に引き上げ・調整のプロンプトが表示され、タスクの再起動不要で継続可能。
- **非対話型実行**: `--max-ai-credits` オプションで単一実行の上限を指定。スクリプトでの利用に最適。

### 注意事項

- セッション制限は**ソフトキャップ** — レスポンス返却後に使用量が判明するため、進行中のレスポンスは完了してから停止。実際の使用量が設定値をわずかに超過する可能性あり。
- セッション制限は1セッションの支出を制御するもので、月次や組織全体の予算・支出制限を補完するが置き換えるものではない。

### 要件

- Copilot CLI 1.0.66 以降
- Copilot SDK 1.0.5 以降
- `copilot update` コマンドで更新可能

### 対象プラン

Copilot for Individuals、Business、Enterprise（パブリックプレビュー）

## 参考リンク

- [Set AI credit session limits in Copilot CLI and SDK](https://github.blog/changelog/2026-07-01-set-ai-credit-session-limits-in-copilot-cli-and-sdk/)
