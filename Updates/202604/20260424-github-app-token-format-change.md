# GitHub App インストールトークンの新フォーマットに関する予告

## 日付

2026-04-24

## ステータス

予告

## 概要

2026年4月27日以降、GitHub App インストールトークンのフォーマットが段階的に更新されます。トークン長が約520文字に拡大し、ステートレスな JWT ベースのフォーマットに変更されます。Copilot コードレビューフローで使用される user-to-server トークンにも今後影響する予定です。

## 詳細

### 変更内容

- トークンの全体長が約520文字に拡大（データにより可変）
- フォーマットが `ghs_APPID_JWT` に変更（プレフィックス `ghs_` は維持）
- JWT は GitHub 内部発行者による署名付き

### 対象範囲

- GitHub Enterprise Cloud およびデータレジデンシー環境が対象
- GitHub Enterprise Server は対象外
- GitHub App インストール server-to-server トークン（Actions GITHUB_TOKEN を含む）が対象
- Copilot コードレビューフローで使用される user-to-server トークンは今後別途発表予定

### ロールアウトスケジュール

1. **4月27日〜5月中旬**: Actions の GITHUB_TOKEN とファーストパーティ統合（Dependabot、Slack、Teams）に段階的適用
2. **5月中旬〜6月下旬**: 全 GitHub App インストールトークンに段階的適用。ブラウンアウト期間を設けて影響確認

### 準備事項

- トークンを不透明な文字列として扱い、ハードコードされたパターンによるバリデーションを避ける
- `ghs_[A-Za-z0-9]{36}` などの正規表現を見直す
- データベースのトークンカラムが520文字以上に対応しているか確認する

## 参考リンク

- [Notice about upcoming new format for GitHub App installation tokens](https://github.blog/changelog/2026-04-24-notice-about-upcoming-new-format-for-github-app-installation-tokens)
- [GitHub App インストールトークン ドキュメント](https://docs.github.com/apps/creating-github-apps/authenticating-with-a-github-app/authenticating-as-a-github-app-installation)
