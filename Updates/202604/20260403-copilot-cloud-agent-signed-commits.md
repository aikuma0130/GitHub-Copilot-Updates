# Copilot cloud agent がコミットに署名を付与

## 日付

2026-04-03

## ステータス

GA

## 概要

Copilot cloud agent が作成するすべてのコミットに署名が付与されるようになりました。これにより「署名済みコミットの必須化」ブランチ保護ルールが有効なリポジトリでもエージェントが利用可能になります。

## 詳細

Copilot cloud agent が作成するコミットに自動的に署名が付与され、GitHub 上で `Verified` バッジが表示されるようになりました。

### 主な改善点

- **コミットの信頼性向上**: 署名付きコミットにより、コミットがエージェントによって作成され改ざんされていないことを確認可能
- **ブランチ保護ルールとの互換性**: 「Require signed commits」ブランチ保護ルールまたはルールセットが有効なリポジトリでも Copilot cloud agent が利用可能に
- 従来はこのルールに準拠できず、該当リポジトリではエージェントの使用がブロックされていた

## 参考リンク

- [Copilot cloud agent signs its commits](https://github.blog/changelog/2026-04-03-copilot-cloud-agent-signs-its-commits)
- [About Copilot cloud agent](https://docs.github.com/copilot/concepts/agents/coding-agent/about-coding-agent)
