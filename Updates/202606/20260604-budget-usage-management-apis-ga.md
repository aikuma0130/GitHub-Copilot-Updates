# 予算・使用量管理 API が一般提供開始

## 日付

2026-06-04

## ステータス

GA

## 概要

GitHub の課金 API が拡張され、予算のプログラム管理、使用量の追跡、コストセンターデータへのアクセスが一般提供開始。API 経由で予算のライフサイクル全体を管理可能に。

## 詳細

### 予算管理 API

- 予算の作成・更新・削除をプログラムで実行可能に（従来は UI のみ）
- 予算額の調整とアラート通知の設定
- 現時点でアカウントあたり最大50予算の一時的な制限あり

### 使用量サマリー API

- アカウント全体またはフィルタ（組織、リポジトリ、コストセンター、製品、SKU）別に使用量情報を取得可能
- 年、月、日単位でクエリ可能

### 利用可能なユーザー

- GitHub Enterprise プランのエンタープライズオーナーおよび課金マネージャー
- GitHub Team プランの組織オーナー
- 個人プランのユーザー

## 参考リンク

- [Budget and usage management APIs now generally available](https://github.blog/changelog/2026-06-04-budget-and-usage-management-apis-now-generally-available/)
