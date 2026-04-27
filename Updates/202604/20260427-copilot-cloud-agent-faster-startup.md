# Copilot cloud agent が Actions カスタムイメージにより 20% 高速起動

## 日付

2026-04-27

## ステータス

Improvement

## 概要

Copilot cloud agent が GitHub Actions カスタムイメージによる最適化されたランナー環境を活用し、起動時間が 20% 以上短縮されました。

## 詳細

### 改善内容

[Copilot cloud agent](https://docs.github.com/copilot/concepts/agents/coding-agent/about-coding-agent) の起動時間が 20% 以上短縮されました。[GitHub Actions カスタムイメージ](https://docs.github.com/actions/using-github-hosted-runners/using-larger-runners/managing-larger-runners#configuring-a-custom-image)を使用して環境を事前構築することで、起動のオーバーヘッドが大幅に削減されています。

### 対象となる操作

Issue を Copilot に割り当てたとき、**Agents** タブからタスクを開始したとき、またはプルリクエストで `@copilot` をメンションしたときに、クラウドベースの環境がより迅速に起動します。

### 累積的な改善

この改善は [3月に出荷された 50% の起動時間短縮](https://github.blog/changelog/2026-03-19-copilot-coding-agent-now-starts-work-50-percent-faster/)に加えた追加の最適化であり、Copilot cloud agent を使用する際のフィードバックループをさらに短縮します。

## 参考リンク

- [Copilot cloud agent starts 20% faster with Actions custom images](https://github.blog/changelog/2026-04-27-copilot-cloud-agent-starts-20-faster-with-actions-custom-images)
- [Copilot cloud agent ドキュメント](https://docs.github.com/copilot/concepts/agents/coding-agent/about-coding-agent)
