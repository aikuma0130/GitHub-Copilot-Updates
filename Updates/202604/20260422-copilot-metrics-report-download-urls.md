# Copilot 利用メトリクスレポートのダウンロード URL 変更予告

## 日付

2026-04-22

## ステータス

予告（2026年5月20日より適用）

## 概要

Copilot 利用メトリクスレポートのダウンロード URL が Azure Front Door ドメインから GitHub 所有のカスタムドメイン（`copilot-reports.github.com`）に移行されます。ファイアウォールやプロキシの許可リスト更新が必要です。

## 詳細

### 変更内容

2026年5月20日より、Copilot Usage Metrics API が返すレポートダウンロードリンクのドメインが変更されます。

**github.com（GHEC）のお客様：**

| | 現在 | 新しい形式 |
|---|---|---|
| ダウンロード URL パターン | `https://copilot-reports-*.b01.azurefd.net/...` | `https://copilot-reports.github.com/...` |

**ghe.com のお客様：**

| | 現在 | 新しい形式 |
|---|---|---|
| ダウンロード URL パターン | `https://copilot-reports-*.b01.azurefd.net/...` | `https://copilot-reports.*.ghe.com/...` |

### 必要な対応

ファイアウォールやプロキシの許可リストを使用している組織は、2026年5月20日までに以下のドメインを追加してください：

- **github.com:** `https://copilot-reports.github.com`
- **ghe.com:** `https://copilot-reports.*.ghe.com`

レガシーの `copilot-reports-*.b01.azurefd.net` パターンは移行期間中引き続き動作しますが、最終的に廃止されます。

### 変更の理由

- レポートダウンロード URL がインフラ変更に関わらず一定に保たれる
- エンタープライズセキュリティチームが予測可能で信頼性の高いドメインを許可リストに設定可能
- 自動化スクリプトや統合がドメイン変更により中断されない

## 参考リンク

- [Upcoming change to Copilot usage metrics report download URLs](https://github.blog/changelog/2026-04-22-upcoming-change-to-copilot-usage-metrics-report-download-urls/)
- [Copilot allowlist reference](https://docs.github.com/copilot/reference/copilot-allowlist-reference)
