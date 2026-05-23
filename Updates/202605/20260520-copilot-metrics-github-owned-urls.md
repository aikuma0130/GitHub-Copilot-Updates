# Copilot 使用量メトリクスレポートのダウンロード URL が GitHub 所有ドメインに移行

## 日付

2026-05-20

## ステータス

GA

## 概要

Copilot 使用量メトリクスレポートのダウンロード URL が Azure Front Door ドメインから GitHub 所有のカスタムドメイン（`copilot-reports.github.com`）に移行された。URL の安定性が向上し、エンタープライズ顧客のファイアウォール・プロキシ許可リスト管理が容易に。

## 詳細

### 変更内容

Copilot Usage Metrics API が返すレポートダウンロードリンクが新しいドメインを使用するようになった。

**github.com (GHEC) 顧客:**

| 項目 | 旧 | 新 |
|------|----|----|
| URL パターン | `https://copilot-reports-*.b01.azurefd.net/...` | `https://copilot-reports.github.com/...` |

**ghe.com 顧客:**

| 項目 | 旧 | 新 |
|------|----|----|
| URL パターン | `https://copilot-reports-*.b01.azurefd.net/...` | `https://copilot-reports.*.ghe.com/...` |

### 必要な対応

ファイアウォールまたはプロキシ許可リストを使用している場合、以下のドメインを追加する：

- **github.com:** `https://copilot-reports.github.com`
- **ghe.com:** `https://copilot-reports.SUBDOMAIN.ghe.com`

レガシーの `copilot-reports-*.b01.azurefd.net` パターンは移行期間中引き続き動作するが、最終的に非推奨化される予定。

### 変更の理由

以前の Azure Front Door ドメインはインフラ固有であり、サービスの再デプロイ・再構成時に変更される可能性があった。GitHub 所有ドメインへの移行により、URL の恒常性・信頼性・自動化スクリプトの安定性が確保される。

## 参考リンク

- [Copilot usage metrics reports now use GitHub-owned download URLs](https://github.blog/changelog/2026-05-20-copilot-usage-metrics-reports-now-use-github-owned-download-urls/)
- [Copilot allowlist reference](https://docs.github.com/copilot/reference/copilot-allowlist-reference)
