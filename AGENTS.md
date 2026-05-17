# AGENTS.md

このフォルダは、Codex と Claude Code が共有するローカル共通メモリです。

## First Step

作業を始める前に、可能な範囲で以下を確認してください。

1. `/Users/satotowa/ai-memory/START_HERE.md`
2. `/Users/satotowa/ai-memory/AI_MEMORY.md`
3. `/Users/satotowa/ai-memory/02_Decisions.md`
4. `/Users/satotowa/ai-memory/03_Preferences.md`
5. `/Users/satotowa/ai-memory/01_Current-Projects.md`

## Source of Truth

共通メモリの正本は `/Users/satotowa/ai-memory` です。
このパスは Google Drive for desktop の同期フォルダを指すシンボリックリンクです。

GitHub `https://github.com/zosuntowa-a11y/ai-memory` は、必要に応じた手動バックアップ・履歴管理用です。

## Response Style

- 日本語で返答する。
- 最初に結論とおすすめを伝える。
- 実務的に、でも少し柔らかく話す。
- 選択肢は 2〜3 個に絞る。

## Memory Update

会話や作業の最後に、必要に応じて以下の形式で更新案を出してください。

```markdown
### 追加する前提
-

### 決定事項
-

### 未解決事項
-

### 次のアクション
-
```

保存対象は、今後も使う前提・決定事項・好みや方針・継続中プロジェクトに絞ってください。
雑談、一時的な作業、その場限りの細かい内容は原則として保存しません。

共通メモリを変更する場合は、原則として `main` に直接 push せず、更新用ブランチを作成して Pull Request で変更提案してください。
PR をマージした後は、ローカル正本 `/Users/satotowa/ai-memory` で `git pull` して、Google Drive 同期フォルダ側へ反映してください。
