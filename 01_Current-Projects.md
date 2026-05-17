# Current Projects

## AI 共通メモリ基盤（運用フェーズ）

### Goal
Claude / ChatGPT / Codex / Claude Code が同じ前提で動けるよう共通メモリを一元管理し、会話で得た要点を蓄積して、AI の前提を自分好みに育てていく。

### 現在の構成（2026-05-18 時点）
- 正本: `/Users/satotowa/ai-memory`（Google Drive for desktop の同期フォルダ）
- バックアップ・履歴管理: GitHub `https://github.com/zosuntowa-a11y/ai-memory`
- Claude Code: `/Users/satotowa/CLAUDE.md` により自動読み込み
- Codex: `AGENTS.md` / `CODEX_INSTRUCTIONS.md` を参照
- ChatGPT: GitHub App「ChatGPT Codex Connector」で ai-memory に接続済み（読み書き可・ai-memory のみにスコープ）

### メモリ更新フロー（半自動）
1. 会話の節目で、会話から重要事項を抽出して更新案を作成する。
2. 更新用ブランチを作成し、Pull Request で変更提案を出す（`main` 直 push はブランチ保護で不可）。
3. 人間 または Claude Code が PR をレビューしてマージする。
4. マージ後、ローカル `/Users/satotowa/ai-memory` で `git pull` し、正本へ反映する（Google Drive が自動同期）。

### 運用上の習慣
- 貯める: 会話の節目で更新案を作り、PR にする。
- 整理する: 月1回ほど棚卸しする（重複の統合・古い情報の削除・見出し整理）。貯めるだけだとノイズが増えて使いにくくなるため。

### 未解決・要対応
- 過去に GitHub トークンをチャットに貼ってしまった件。push は SSH 鍵方式へ移行済みでトークンは使わなくなったが、流出したトークン自体が未失効の場合は GitHub の Developer settings で失効させる必要がある。
