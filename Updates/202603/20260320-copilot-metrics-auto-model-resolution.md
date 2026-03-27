# Copilot 利用メトリクスで自動モデル選択を実際のモデル名に解決

## 日付

2026-03-20

## ステータス

GA

## 概要

自動モデル選択時に「Auto」と表示されていた利用データが、実際に使用されたモデル名に解決されるようになり、管理者が正確なモデル使用状況を把握できるようになりました。

## 詳細

Copilot 利用メトリクスで、自動モデル選択が有効な場合のモデル使用状況が完全に明確化されました。

以前は「Auto」ラベルで表示されていたアクティビティが、実際のモデル名に解決されるようになりました。REST API と ダッシュボードの両方で、`totals_by_model_feature`（Enterprise、Org、User レベル）および「Model usage per chat mode」チャートに適用されます。

## 参考リンク

- [Copilot usage metrics now resolve auto model selection to actual models](https://github.blog/changelog/2026-03-20-copilot-usage-metrics-now-resolve-auto-model-selection-to-actual-models)
