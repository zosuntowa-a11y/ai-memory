# AI Memory

このファイルは、Claude / ChatGPT / Codex / Claude Code が共通メモリを確認するときの短い要約です。
詳しい入口は `START_HERE.md` を確認します。

## Project Goal

Claude、ChatGPT、Codex、Claude Code を並行して使うための共通メモリ運用を整える。
Google Drive for desktop で同期されるローカルMarkdownフォルダを長期記憶の正本として使い、各 AI に必要な前提を呼び出せるようにする。
GitHub は必要に応じた手動バックアップ・履歴管理用として扱う。
Obsidian はこのフォルダを編集・整理しやすくする補助UIとして使う。

## Current Status

- 共通メモリの正本は `/Users/satotowa/ai-memory`。
- 実体は Google Drive 個人アカウント側の同期フォルダにある。
- GitHub `https://github.com/zosuntowa-a11y/ai-memory` は手動バックアップ・履歴管理用。
- `START_HERE.md` を、各 AI が最初に読む入口として使う。
- 各 AI の固定指示に「質問に答える前に、可能な範囲で共通メモリを確認する」と書く。

## Decisions

- Google Drive 同期フォルダを全体の共通メモリの正本として使う。
- Obsidian は編集・整理用の補助UIとして使う。
- GitHub は必須ではなく、必要なときだけ手動バックアップとして使う。
- 会話の最後に、必要に応じて「共通メモリ更新案」を AI に作らせる。
- 全会話ログではなく、次回以降に必要な要約だけを残す。

## Style Preferences

- 日本語で、実務的かつ柔らかいトーン。
- まず結論とおすすめを示す。
- 選択肢が多い場合は、2〜3個に絞る。
- 長期保存するメモリは、短く、検索しやすく、あとで読み返しやすい形にする。

## Next Actions

- `/Users/satotowa/CLAUDE.md` からこのフォルダを参照して Claude Code に読ませる。
- Codex は作業開始時に `/Users/satotowa/ai-memory/START_HERE.md` を読む。
- `CHATGPT_CUSTOM_INSTRUCTIONS.md` や `CLAUDE_PROJECT_INSTRUCTIONS.md` は必要になった場合だけ使う。
- 重要な決定は `02_Decisions.md` に集約する。
