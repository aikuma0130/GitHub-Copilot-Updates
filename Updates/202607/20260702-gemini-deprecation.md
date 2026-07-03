# Gemini 2.5 Pro および Gemini 3 Flash の非推奨化予告

## 日付

2026-07-02

## ステータス

Deprecated (2026年7月31日に廃止予定)

## 概要

Gemini 2.5 Pro と Gemini 3 Flash が2026年7月31日に全 Copilot エクスペリエンスで非推奨となる。代替としてそれぞれ Gemini 3.1 Pro、Gemini 3.5 Flash への移行が推奨される。

## 詳細

GitHub Copilot の全エクスペリエンス（Copilot Chat、インライン編集、ask/agent モード、コード補完を含む）において、以下のモデルが2026年7月31日に廃止される。

| モデル | 廃止日 | 推奨代替モデル |
|--------|--------|----------------|
| Gemini 2.5 Pro | 2026-07-31 | Gemini 3.1 Pro |
| Gemini 3 Flash | 2026-07-31 | Gemini 3.5 Flash |

### 必要なアクション

- 廃止日までにワークフローとインテグレーションを代替モデルに更新すること
- Copilot Enterprise 管理者は、Copilot 設定のモデルポリシーで代替モデルへのアクセスを有効にする必要がある場合がある
- 古いモデルは廃止後に自動的に削除されるため、削除のためのアクションは不要

## 参考リンク

- [Upcoming deprecation of Gemini 2.5 Pro and Gemini 3 Flash](https://github.blog/changelog/2026-07-02-upcoming-deprecation-of-gemini-2-5-pro-and-gemini-3-flash/)
- [Copilot で利用可能なモデル一覧](https://docs.github.com/copilot/reference/ai-models/supported-models)
