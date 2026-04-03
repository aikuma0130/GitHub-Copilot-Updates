# Copilot cloud agent の Organization ランナー制御

## 日付

2026-04-03

## ステータス

GA

## 概要

Organization 管理者が Copilot cloud agent で使用するランナーを Organization 全体でデフォルト設定およびロックできるようになりました。リポジトリごとの個別設定が不要になり、一貫したランナーポリシーの展開が可能です。

## 詳細

Copilot cloud agent はタスクごとに GitHub Actions を利用した新しい開発環境を起動します。従来はリポジトリレベルの `copilot-setup-steps.yml` でランナーを設定する必要がありましたが、Organization 全体での統一的なデフォルト設定やガードレールの適用が困難でした。

### 新機能

- **デフォルトランナーの設定**: Organization 内のすべてのリポジトリで自動的に使用されるデフォルトランナーを設定可能。個別リポジトリの設定は不要
- **ランナー設定のロック**: 個別リポジトリが Organization のデフォルトを上書きできないようにロック可能

### ユースケース

- より大きな GitHub Actions ランナーを使用してパフォーマンスを向上
- セルフホストランナーを指定してエージェントの実行場所を統制
- チーム全体に一貫したデフォルト設定を展開

## 参考リンク

- [Organization runner controls for Copilot cloud agent](https://github.blog/changelog/2026-04-03-organization-runner-controls-for-copilot-cloud-agent)
- [Configuring runners for GitHub Copilot cloud agent in your organization](https://docs.github.com/copilot/how-tos/administer-copilot/manage-for-organization/configure-runner-for-coding-agent)
