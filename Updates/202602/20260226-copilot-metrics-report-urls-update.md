# Copilot メトリクスレポート URL の更新

## 日付

2026-02-26

## ステータス

Improvement

## 概要

Copilot 使用メトリクス API のダウンロード URL エンドポイントが変更。ファイアウォール設定の更新が必要な場合あり。

## 詳細

Copilot 使用メトリクス API のダウンロード URL が新しいエンドポイントに変更されました。レポートデータ、API コントラクト、レスポンススキーマに変更はありません。ファイアウォールで CDN ドメインを許可している場合は、`copilot-reports-production-*.b01.azurefd.net` を追加する必要があります。

## 参考リンク

- [Copilot metrics report URLs update](https://github.blog/changelog/2026-02-26-copilot-metrics-report-urls-update)
