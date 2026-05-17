# Decisions

## 2026-05-11

- 当初は GitHub（zosuntowa-a11y/ai-memory）を共通メモリの正本として使う方針だった。
- AI サービス内の記憶には頼りすぎず、外部のユーザー管理レイヤーに共通メモリを置く。
- 会話ログは丸ごと保存しない。次の会話に必要な要点だけを残す。
- 各 AI には会話の終わりに「共通メモリ更新案」を出してもらう。
- AI の役割分担：Claude（発想・壁打ち）/ ChatGPT（説明・整理）/ Codex（ファイル・コード）。
- 各 AI の固定指示には「質問に答える前に、可能な範囲で `START_HERE.md` と関連メモリを確認する」と書く。
- Claude Code 用に `CLAUDE.md` を用意する。
- 現在方針：共通メモリの正本は GitHub ではなく、Google Drive for desktop で同期される `/Users/satotowa/ai-memory` にする。
- GitHub は必須ではなく、必要に応じた手動バックアップ・履歴管理用にする。
