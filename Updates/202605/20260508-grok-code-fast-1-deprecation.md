# Grok Code Fast 1 の非推奨化予告

## 日付

2026-05-08

## ステータス

Deprecated（2026-05-15 非推奨化予定）

## 概要

Grok Code Fast 1 が 2026年5月15日に全 Copilot エクスペリエンスで非推奨化されます。モデルプロバイダー側の廃止に伴い前倒しスケジュールとなっており、代替として GPT-5 mini / Claude Haiku 4.5 が推奨されています。

## 詳細

### 非推奨化の詳細

| モデル | 非推奨化日 | 推奨代替モデル |
|---|---|---|
| Grok Code Fast 1 | 2026-05-15 | GPT-5 mini / Claude Haiku 4.5 |

### 前倒しの理由

モデルプロバイダー（xAI）による 2026年5月15日のモデル廃止に伴い、通常より前倒しのスケジュールで非推奨化が実施されます。

### 影響範囲

以下の全 Copilot エクスペリエンスが対象です：

- Copilot Chat
- インライン編集
- Ask モードおよび Agent モード
- コード補完

### 必要な対応

- ワークフローと統合をサポート対象モデル（GPT-5 mini / Claude Haiku 4.5）に更新してください
- Copilot Enterprise 管理者は、Copilot 設定のモデルポリシーで代替モデルへのアクセスを有効化する必要がある場合があります
- 管理者は個人の Copilot 設定でモデルの利用可否を確認し、ポリシーが有効化されていることを確認できます
- 非推奨化されたモデルの削除について追加の対応は不要です

## 参考リンク

- [Upcoming deprecation of Grok Code Fast 1](https://github.blog/changelog/2026-05-08-upcoming-deprecation-of-grok-code-fast-1/)
- [xAI モデル廃止情報](https://docs.x.ai/developers/migration/may-15-retirement)
- [Copilot で利用可能なモデル一覧](https://docs.github.com/copilot/reference/ai-models/supported-models)
