# AI Memory

このファイルは、Claude / ChatGPT / Codex / Claude Code が共通メモリを確認するときの短い要約です。
詳しい入口は `START_HERE.md` を確認します。

## Project Goal

Claude、ChatGPT、Codex、Claude Code を並行して使うための共通メモリ運用を整える。
GitHub を長期記憶の正本として使い、各 AI に必要な前提を呼び出せるようにする。
Obsidian は人間が編集・整理しやすい補助ノートとして使う。

## Current Status

- 共通メモリの正本は GitHub `https://github.com/zosuntowa-a11y/ai-memory`。
- `START_HERE.md` を、各 AI が最初に読む入口として使う。
- 各 AI の固定指示に「質問に答える前に、可能な範囲で共通メモリを確認する」と書く。

## Decisions

- GitHub を全体の共通メモリの正本として使う。
- Obsidian は編集・整理用の補助ノートとして使う。
- 会話の最後に、必要に応じて「共通メモリ更新案」を AI に作らせる。
- 全会話ログではなく、次回以降に必要な要約だけを残す。

## Style Preferences

- 日本語で、実務的かつ柔らかいトーン。
- まず結論とおすすめを示す。
- 選択肢が多い場合は、2〜3個に絞る。
- 長期保存するメモリは、短く、検索しやすく、あとで読み返しやすい形にする。

## Next Actions

- `CHATGPT_CUSTOM_INSTRUCTIONS.md` を ChatGPT のカスタム指示に使う。
- `CLAUDE_PROJECT_INSTRUCTIONS.md` を Claude の Project Instructions に使う。
- `CLAUDE.md` を Claude Code 用のリポジトリ指示に使う。
- 重要な決定は `02_Decisions.md` に集約する。

