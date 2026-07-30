# Copilot Business / Enterprise 向けモデルのデフォルト有効化ポリシー

## 日付

2026-07-29

## ステータス

GA

## 概要

Copilot Business および Enterprise プランで、GA モデルがデフォルトで有効化されるグローバルポリシーが導入された。管理者が新モデルを個別に有効化する手間が不要となり、オプトアウト制御で厳格なガバナンスにも対応。

## 詳細

### 変更内容

- 新たに「リリース済みモデルのデフォルト利用可否」ポリシーがエンタープライズおよび組織のモデル設定に追加。
- ポリシーは本日（7月29日）から設定可能だが、28日間はモデルの利用可否に影響しない。

### ポリシー発効（8月26日）

- 明示的に設定されていないモデルは「unconfigured」から「inherits default」にラベルが変更され、ポリシー設定に従って利用可否が決定される。
- ポリシーが有効（デフォルト）の場合、対象モデルがユーザーに利用可能になる。無効に設定した場合はオフのまま。
- 「inherits default」はポリシーに動的に追従するライブ状態。ポリシーの切り替えは即時反映される。
- 管理者が明示的に有効化・無効化したモデルの設定は一切変更されない。

### 除外モデル

- オープンウェイトモデル（DeepSeek、Kimi K2.7 等）およびデータ保持契約の対象外モデル（Fable 5 等）は、ポリシー設定にかかわらずデフォルト有効化の対象外。

### 推奨アクション

- 8月26日までにモデル設定を確認し、モデルがデフォルトで利用可能になることに問題がなければ対応不要。
- 各モデルを手動で承認したい場合は、8月26日までにポリシーを `disabled` に設定する。

## 参考リンク

- [Default model enablement for Copilot Business and Enterprise](https://github.blog/changelog/2026-07-29-default-model-enablement-for-copilot-business-and-enterprise/)
- [About default availability of Copilot models](https://docs.github.com/en/copilot/concepts/models/default-availability)
