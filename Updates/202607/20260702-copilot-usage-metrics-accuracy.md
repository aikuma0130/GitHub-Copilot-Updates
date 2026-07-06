# Copilot 使用メトリクスレポートの精度とカバレッジ向上

## 日付

2026-07-02

## ステータス

GA

## 概要

Copilot 使用メトリクス API のデータ精度とカバレッジが向上。CLI の提案行数レポート、IDE 識別の改善、AI クレジット帰属の正確化により、組織全体の利用状況をより正確に把握可能に。

## 詳細

### 主な改善点

#### Copilot CLI の提案行数レポート

GitHub Copilot CLI が提案するコード行数を `loc_suggested_to_add_sum` および `loc_suggested_to_delete_sum` フィールドに報告するようになった。以前はこれらのフィールドは CLI 利用時に常に 0 を返していた。また、新しい CLI バージョンでは重複編集が複数回カウントされなくなり、コード生成カウントがより正確になった。

#### IDE 識別の改善

サーバーサイドテレメトリのみで確認されていたユーザーの IDE とプラグインバージョンが報告されるようになった。`totals_by_ide` メトリクスがより多くの Copilot ユーザーを反映し、実際の使用パターンをより正確に表現する。

#### AI クレジット帰属の正確化

以下の2つの問題が修正された：
- 組織に紐付けられていない消費が以前は除外されていたが、適切に割り当てられるようになった
- サーバーサイドテレメトリのみで追跡されるユーザーの AI クレジット消費が請求データに含まれるようになった

### 要件

- 提案行数の完全な機能には CLI v1.0.57 以降が必要
- コード生成の重複排除には CLI v1.0.64 以降が必要
- エンタープライズ管理者およびオーガニゼーションオーナーが REST API で利用可能

## 参考リンク

- [Improved accuracy and coverage in Copilot usage metrics reports](https://github.blog/changelog/2026-07-02-improved-accuracy-and-coverage-in-copilot-usage-metrics-reports/)
