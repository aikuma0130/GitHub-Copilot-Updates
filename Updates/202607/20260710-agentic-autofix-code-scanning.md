# Code Scanning アラートのエージェント型自動修正がパブリックプレビュー

## 日付

2026-07-10

## ステータス

Public Preview

## 概要

Code Scanning アラートに対するエージェント型自動修正（Agentic Autofix）がパブリックプレビューとして提供開始。Copilot がコードベースを探索し、修正を提案し、CodeQL で検証した上で PR を作成する。

## 詳細

### 動作の仕組み

Code Scanning アラートを Copilot に割り当てると、以下のプロセスが実行される:

1. コードベース内の関連ファイルを探索
2. 修正案を生成
3. CodeQL を再実行して修正がアラートを解消することを検証
4. 必要に応じて反復し、ドラフト PR を作成

修正生成は通常2〜4分で完了。PR には修正の概要、アラート解消の理由、検証ステップが含まれる。

### トリガー方法

- 個別の Code Scanning アラートから Copilot に割り当て
- セキュリティアラート一覧から複数アラートを選択して一括修正
- セキュリティキャンペーン内での一括修正
- REST API で `assignees` を `["copilot-swe-agent[bot]"]` に設定

### 前提条件

- GitHub Code Security または GitHub Advanced Security ライセンス
- Copilot cloud agent が有効な Copilot ライセンス

### 課金

- パブリックプレビュー期間中は組織の AI クレジットを消費
- GitHub Actions 分数も消費される

## 参考リンク

- [Agentic autofix for code scanning alerts in public preview](https://github.blog/changelog/2026-07-10-agentic-autofix-for-code-scanning-alerts-in-public-preview/)
- [Copilot usage-based billing](https://docs.github.com/enterprise-cloud@latest/copilot/concepts/billing/usage-based-billing-for-organizations-and-enterprises)
