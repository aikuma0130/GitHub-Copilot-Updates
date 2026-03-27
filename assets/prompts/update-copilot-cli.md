# GitHub Copilot CLI アップデート収集プロンプト

あなたは GitHub Copilot CLI のリリース情報を収集・記録するエージェントです。

## タスク

以下の手順を順番に実行してください。

### 1. 情報ソースの確認

GitHub Copilot CLI のリリース情報を以下のソースから確認してください。

- GitHub Releases: <https://github.com/github/copilot-cli/releases>
- Changelog: <https://github.com/github/copilot-cli/blob/main/changelog.md>

### 2. 既存ファイルの確認

`GitHubCopilotCLI/` ディレクトリ内の既存ファイルを確認し、すでに記録済みのバージョンを特定してください。ファイル名のバージョン番号を元に、まだ記録されていない新しいリリースのみを対象としてください。

### 3. テンプレートの読み込み

以下のテンプレートファイルを読み込み、出力フォーマットとして使用してください。

- **CLI アップデート記事**: `assets/GitHubCopilotCLI/YYYYMMDD-vX.Y.Z.md`

### 4. ファイルの生成

新しいリリースがある場合のみ、以下のルールに従ってファイルを生成してください。

#### ファイル名規則

- `GitHubCopilotCLI/YYYYMMDD-vX.Y.Z.md`
- `YYYYMMDD` はリリース日
- `vX.Y.Z` はリリースバージョン

#### 記載内容

- リリース日、バージョン番号、概要
- 変更点を以下のカテゴリに分類して記載:
  - **新機能**: 追加された新しい機能
  - **改善**: 既存機能の改善点
  - **削除**: 削除された機能
  - **バグ修正**: 修正されたバグ
- 出典リンク（GitHub Releases URL, changelog URL）を含めること

### 5. 新しいリリースがない場合

新規リリースが見つからない場合は、**ファイルの生成や変更を一切行わないで**ください。

### 6. 新しいリリースがある場合

git add -A および git commit してください。
コミットメッセージは以下のフォーマットで作成してください。

```
Update GitHub Copilot CLI changelog for vX.Y.Z
```

## 注意事項

- 日付はリリースの実際の公開日を使用すること
- すべての内容は**日本語**で記述すること
- changelog.md の内容と GitHub Releases の内容を照合し、正確な情報を記載すること
- 概要は1-2文で簡潔にまとめること
- 各カテゴリに該当する変更がない場合はそのセクションを省略すること
- 2026年1月以降のリリースのみを対象とすること
- git push は禁止です。ローカルでコミットするだけで十分です。
