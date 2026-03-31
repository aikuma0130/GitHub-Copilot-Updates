# GitHub Issues と Projects でエージェントアクティビティを表示

## 日付

2026-03-26

## ステータス

GA

## 概要

Copilot などの coding agent が Issue に割り当てられた際、セッション状態が Issue のサイドバーやプロジェクトのテーブル・ボードビューに直接表示されるようになりました。

## 詳細

GitHub Issues と Projects に、エージェントアクティビティを直接統合する2つの新機能がリリースされました。

### Issue のアサイニー配下にエージェントセッションを表示

coding agent（Copilot、Claude、Codex など）が Issue に割り当てられると、セッションがサイドバーのアサイニー配下に表示されます。各セッションには「queued」「working」「waiting for review」「completed」のライブステータスが表示され、クリックするとセッションログに直接ジャンプできます。

この機能は、coding agent にアクセスできるすべてのリポジトリで一般提供（GA）されています。

### プロジェクトのテーブル・ボードビューにエージェントセッションを表示

エージェントセッションがプロジェクトのテーブルビューおよびボードビューにも表示されるようになりました。どのアイテムにエージェントセッションが紐づいているか、現在のステータス、大量の作業の進捗状況を一目で確認できます。

表示するには、**View** メニューを開き、**Show agent sessions** をオンにしてください。

## 参考リンク

- [Agent activity in GitHub Issues and Projects](https://github.blog/changelog/2026-03-26-agent-activity-in-github-issues-and-projects)
- [GitHub Community ディスカッション](https://github.com/orgs/community/discussions/190731)
