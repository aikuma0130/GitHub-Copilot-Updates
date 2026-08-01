# Gemini 2.5 Pro および Gemini 3 Flash が廃止

## 日付

2026-07-31

## ステータス

Deprecated

## 概要

Gemini 2.5 Pro と Gemini 3 Flash が全 GitHub Copilot エクスペリエンスで正式に廃止された。代替として Gemini 3.1 Pro および Gemini 3.5 Flash への移行が必要。

## 詳細

2026年7月2日に予告されていた通り、Gemini 2.5 Pro と Gemini 3 Flash が本日付で全 Copilot エクスペリエンス（Copilot Chat、インライン編集、ask/agent モード、コード補完）から削除された。

| モデル | 推奨代替モデル |
|--------|----------------|
| Gemini 2.5 Pro | Gemini 3.1 Pro |
| Gemini 3 Flash | Gemini 3.5 Flash |

### 管理者向けアクション

- Copilot Enterprise 管理者は、代替モデルが Copilot 設定のモデルポリシーで有効化されていることを確認する必要がある
- 有効化後、VS Code および github.com の Copilot Chat モデルセレクターに代替モデルが表示される
- 廃止されたモデルは自動的にセレクターから削除されるため、追加の削除アクションは不要

## 参考リンク

- [Upcoming deprecation of Gemini 2.5 Pro and Gemini 3 Flash](https://github.blog/changelog/2026-07-02-upcoming-deprecation-of-gemini-2-5-pro-and-gemini-3-flash/)
- [Copilot で利用可能なモデル一覧](https://docs.github.com/copilot/reference/ai-models/supported-models)
