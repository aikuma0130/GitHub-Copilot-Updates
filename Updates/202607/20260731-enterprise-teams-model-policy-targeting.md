# エンタープライズチームレベルのモデルポリシーターゲティング（パブリックプレビュー）

## 日付

2026-07-31

## ステータス

Public Preview

## 概要

GitHub Enterprise の Copilot Business/Enterprise ライセンス利用者向けに、チームレベルでモデルアクセスポリシーを設定できる機能がパブリックプレビューとして提供開始。組織レベルではなくチーム単位で細かい制御が可能に。

## 詳細

AI 管理者がエンタープライズ全体のベースラインモデルを設定した上で、特定のエンタープライズチームに追加モデルへのアクセスを付与できるようになった。これにより、職種やフロンティアチームによる先行実験に応じたアクセス制御が可能になる。

### モデルの設定オプション

エンタープライズレベルでモデルを以下のように設定可能：

- **Enabled**: エンタープライズ全メンバーが利用可能
- **Disabled**: エンタープライズ全メンバーが利用不可
- **Optional**: エンタープライズチームに割り当て可能

### 評価ルール

モデルアクセスは最小制限（least-restrictive）戦略で評価される。ユーザーがいずれかのエンタープライズチームからモデルアクセスを取得した場合、そのユーザーはどこでもそのモデルを利用可能。

### 有効化方法

Copilot ページの「Models」セクションにある「Enterprise teams mode」トグルをオンにすることでプレビューにオプトインできる。有効化後、モデルアクセスはエンタープライズレベルおよびエンタープライズチームを通じて管理され、組織レベルのモデル設定は適用されなくなる。

### ロールアウト

2026年8月3日までに大部分のエンタープライズ顧客がプレビューオプトインにアクセス可能になる予定。

## 参考リンク

- [Enterprise teams model policy targeting in public preview](https://github.blog/changelog/2026-07-31-enterprise-teams-model-policy-targeting-in-public-preview/)
- [エンタープライズでのモデル可用性管理ドキュメント](https://docs.github.com/enterprise-cloud@latest/copilot/how-tos/administer-copilot/manage-for-enterprise/manage-availability-of-default-models)
