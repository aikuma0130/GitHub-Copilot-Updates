# Copilot Code Review: 新しい設定とコントロール

## 日付

2026-06-12

## ステータス

GA

## 概要

組織レベルのランナー設定、コンテンツ除外サポート、カスタムインストラクションの文字数制限撤廃により、Copilot Code Review の構成・制御がより柔軟になった。

## 詳細

### ⚙️ 組織レベルのランナー設定

Copilot Code Review のランナータイプを組織レベルで設定可能になった。これにより、1つの設定をすべてのリポジトリに一括適用でき、個別の設定が不要になる。

- 組織管理者がデフォルトランナー（GitHub ホスト、セルフホスト、大規模ランナー）を全リポジトリに適用可能
- ランナー設定をロックすることで、リポジトリ個別の設定をオーバーライド可能
- Copilot クラウドエージェントにも同一設定が適用される

設定パス: 組織 → **Copilot** → **Runner type** → **Runner type configuration**

### 🛡️ コンテンツ除外サポート

Copilot Code Review がリポジトリ、組織、エンタープライズレベルの Copilot コンテンツ除外設定を尊重するようになった。

- 指定したファイルやディレクトリをレビュー対象から除外可能
- リポジトリ管理者がパスベースのルールで除外パスを設定可能
- チームや組織の境界に合わせたレビュースコープの制御が可能

### 📝 カスタムインストラクションの文字数制限撤廃

従来、`.github` ディレクトリ下の `copilot-instructions.md` や `*.instructions.md` ファイルには 4000 文字の制限があったが、この制限が撤廃された。より詳細で柔軟なカスタムインストラクションが記述可能に。

## 参考リンク

- [Copilot code review: New configurations and controls](https://github.blog/changelog/2026-06-12-copilot-code-review-new-configurations-and-controls/)
- [Copilot content exclusions ドキュメント](https://docs.github.com/en/copilot/how-tos/configure-content-exclusion/exclude-content-from-copilot)
