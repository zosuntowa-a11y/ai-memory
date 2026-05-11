# Current Projects

## AI 共通メモリ基盤（完了）

### Goal
Claude / ChatGPT / Codex が同じ前提で動けるよう、共通メモリをクラウドで管理する。

### Setup（完了済み）
- GitHub リポジトリ: https://github.com/zosuntowa-a11y/ai-memory
- ローカルパス: `/Users/satotowa/Documents/Codex/2026-05-11/claude-gpt-codex-claude-gpt-youtube/AI-Memory/`
- Claude: `/Users/satotowa/CLAUDE.md` により自動読み込み
- ChatGPT / Codex: `05_AI-Instructions.md` のプロンプトを会話開始時に貼り付ける

### メモリ更新の手順
1. ローカルのファイルを編集（Obsidian or テキストエディタ）
2. 以下のコマンドでGitHubに反映：
```
cd "/Users/satotowa/Documents/Codex/2026-05-11/claude-gpt-codex-claude-gpt-youtube/AI-Memory" && git add . && git commit -m "update memory" && git push
```

### 未解決
- ChatGPT の自動接続はまだ手動運用（Custom GPT化で解決可能）
- GitHub トークンをチャットに貼ってしまったため要再発行
