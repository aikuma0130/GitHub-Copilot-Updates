# Copilot Code Review のフィードバックを Cloud Agent で簡単に適用

## 日付

2026-05-19

## ステータス

GA

## 概要

Copilot Code Review の「Implement suggestion」ボタンが「Fix with Copilot」に刷新され、UI ダイアログで適用方法を細かく制御可能に。複数コメントの一括適用にも対応し、レビューフィードバックから修正への引き継ぎがよりスムーズに。

## 詳細

### 個別フィードバックの適用改善

従来の **Implement suggestion** ボタンが **Fix with Copilot** に名称変更され、新しい UI ダイアログが追加された。ダイアログでは以下の操作が可能：

- 変更を現在の PR に直接適用するか、新しい PR を作成するかを選択
- 使用する Copilot モデルの選択
- 追加の指示（インストラクション）の入力

### 複数フィードバックの一括適用

Pull Request Overview コメントにあった **Implement all suggestions** ボタンが **Fix batch with Copilot** に置換された。特定のコメントを選択してバッチとして Copilot Cloud Agent に引き渡すことが可能となり、個別対応に比べて大幅に効率化される。

### 従来からの変更点

以前は「Implement suggestion」クリック時に `@Copilot` をタグしたコメントが自動生成され、新しい PR が作成される動作だった。新しいフローでは、引き渡し前にダイアログで詳細を指定できるため、意図しない変更のリスクが低減する。

## 参考リンク

- [Easily apply Copilot code review feedback with Copilot cloud agent](https://github.blog/changelog/2026-05-19-easily-apply-copilot-code-review-feedback-with-copilot-cloud-agent/)
