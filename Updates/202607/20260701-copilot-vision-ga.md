# Copilot Vision が一般提供開始

## 日付

2026-07-01

## ステータス

GA

## 概要

画像や PDF をチャットプロンプトに直接添付して、Copilot がコードと合わせて視覚的に推論できるようになった。全 Copilot プランで利用可能。

## 詳細

### サポートファイル形式

| タイプ | フォーマット |
|--------|-------------|
| 画像 | JPEG (`.jpg`, `.jpeg`)、PNG (`.png`)、GIF (`.gif`)、WebP (`.webp`) |
| ドキュメント | PDF (`.pdf`) |

### 利用可能な環境

- **VS Code の GitHub Copilot Chat** — ペースト、ドラッグ＆ドロップ、右クリックで画像を添付。ask、plan、agent モードで動作。
- **github.com の Copilot Chat** — 画像や PDF を直接添付可能。
- **GitHub Copilot CLI** — ターミナルで画像パスを指定して添付。

### プラン対応

全 Copilot サブスクライバー（Free、Pro、Pro+、Business、Enterprise）で利用可能。管理者によるポリシー変更やアクション不要。

以前は Copilot Business / Enterprise ユーザーに「Editor Preview Features」ポリシーの有効化が必要だったが、現在はデフォルトで全員に有効。

### データ保持

Copilot Business / Enterprise ユーザーの場合、GitHub はサービス提供のため画像・PDF 添付ファイルを約24時間保持する。

## 参考リンク

- [Copilot vision is generally available](https://github.blog/changelog/2026-07-01-copilot-vision-is-generally-available/)
