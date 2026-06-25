# Free・Student プランのモデル選択方式の変更

## 日付

2026-06-24

## ステータス

GA

## 概要

Copilot Free および Student プランで、Auto モデル選択がデフォルトかつ唯一のモデル選択方式に変更された。手動でのモデル選択は廃止され、タスクごとに最適なモデルが自動選択される。

## 詳細

Copilot Free および Student プランにおいて、モデル選択エクスペリエンスが以下のように変更された。

### Auto モデル選択への一本化

- 手動でのモデル選択が廃止され、「Auto」が唯一のモデル選択方式となった
- Auto モデル選択は、各タスクに対して最適なモデルを動的に選択する
- プラン制限に応じて、複数のモデルファミリーのモデルにアクセス可能

### (Preview) ラベルの廃止

- Microsoft リリースモデルから `(Preview)` ラベルが撤廃された
- Auto モデル選択がモデルルーティングを管理し、継続的な改善がバックグラウンドで行われるため、ラベルによるユーザー判断の誘導が不要に

### 対象プラン

- Copilot Free
- Copilot Student

### サポートされるモデルの詳細

Auto モード対応モデルの一覧は [公式ドキュメント](https://docs.github.com/copilot/reference/ai-models/supported-models#supported-ai-models-in-auto-model-selection) を参照。

## 参考リンク

- [Changes to model selection for Free and Student plans](https://github.blog/changelog/2026-06-24-changes-to-model-selection-for-free-and-student-plans/)
- [Auto model selection のドキュメント](https://docs.github.com/copilot/concepts/models/auto-model-selection)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/198751)
