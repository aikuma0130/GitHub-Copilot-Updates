# Copilot cloud agent をカスタムプロパティで組織単位に有効化

## 日付

2026-04-15

## ステータス

GA

## 概要

Enterprise 管理者が Copilot cloud agent（CCA）のアクセスを組織単位で選択的に有効化できるようになりました。Organization カスタムプロパティを使用した柔軟なポリシー管理が可能です。

## 詳細

### 背景

これまで Enterprise 管理者と AI マネージャーは、Copilot cloud agent（CCA）を「すべて有効」「すべて無効」「各組織に委任」のいずれかでしか制御できませんでした。今回のリリースにより、特定の Organization に対して個別に CCA を有効化できるようになりました。

### 新しい API エンドポイント

CCA を管理するための3つの新しい API エンドポイントが追加されました：

- **`PUT`**: ポリシー状態の設定（Organization 判断、全体有効、全体無効、選択した Organization のみ有効）
- **`POST`**: CCA 有効化リストへの Organization の追加
- **`DELETE`**: Organization の CCA を無効化

### AI Controls ページからの管理

AI Controls 設定ページで、Organization のサブセットに対して CCA を選択的に有効化するポリシーを作成できます。既存のポリシーを維持するためのアクションは不要です。

設定は「Agent」→「Copilot Cloud Agent」→「Enabled for selected organizations」で利用できます。

### 注意事項

カスタムプロパティを使用した CCA の有効化は、設定時に一度だけ評価されます。後からカスタムプロパティが追加・削除・変更されても、CCA の有効/無効は自動的に更新されません。

## 参考リンク

- [Enable Copilot cloud agent via custom properties](https://github.blog/changelog/2026-04-15-enable-copilot-cloud-agent-via-custom-properties)
- [REST API ドキュメント](https://docs.github.com/enterprise-cloud@latest/rest/copilot/copilot-coding-agent-management?apiVersion=2026-03-10)
- [Enterprise での CCA 管理ドキュメント](https://docs.github.com/enterprise-cloud@latest/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-agents/manage-copilot-cloud-agent)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/178247)
