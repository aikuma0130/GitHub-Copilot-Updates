# Code Scanning で AI セキュリティ検出が PR に表示

## 日付

2026-07-14

## ステータス

Public Preview

## 概要

GitHub Code Scanning が AI を活用したセキュリティ検出を PR 上に直接表示。CodeQL がネイティブにサポートしていない言語やフレームワークにも脆弱性検出範囲を拡大する。

## 詳細

### 機能概要

AI セキュリティ検出は、GitHub の AI 検出エンジンを活用して CodeQL の対応範囲を拡張する。PR のオープンまたは更新時に自動的にdiff を分析し、ほぼリアルタイムでフィードバックを提供する。

### 主な特徴

- **幅広い言語サポート**: CodeQL が直接サポートしない言語やフレームワークもカバーし、盲点を削減
- **PR へのネイティブ統合**: 検出結果が PR 上に直接表示され、既存のワークフローに自然に統合
- **AI ラベリング**: AI 生成のアラートは「AI」ラベルで明示され、通常の CodeQL 結果と区別可能
- **アドバイザリ性質**: 検出結果は情報提供であり、マージをブロックしない

### 有効化要件

- GitHub Code Security (Advanced Security) が有効であること
- CodeQL のデフォルトセットアップが有効であること
- エンタープライズオーナーによるポリシー許可
- Copilot ライセンスが必要

### 課金

パブリックプレビュー期間中、AI セキュリティ検出の実行時にのみ組織の AI クレジットを消費する。検出結果が生成されない場合は課金されない。

## 参考リンク

- [Code scanning shows AI security detections on pull requests](https://github.blog/changelog/2026-07-14-code-scanning-shows-ai-security-detections-on-pull-requests/)
- [AI-powered security detections in pull requests - GitHub Docs](https://docs.github.com/en/enterprise-cloud@latest/code-security/concepts/code-scanning/ai-powered-security-detections)
