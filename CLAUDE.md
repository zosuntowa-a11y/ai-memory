# CLAUDE.md

このリポジトリは、Claude / ChatGPT / Codex / Claude Code で共有するための共通メモリです。

## Default First Step

作業を始める前に、可能なら以下を確認してください。

1. `START_HERE.md`
2. `AI_MEMORY.md`
3. `02_Decisions.md`
4. `03_Preferences.md`
5. `01_Current-Projects.md`

その上で、ユーザーの最新の依頼を優先して作業してください。

## Purpose

AI サービス内の記憶に頼りすぎず、GitHub 上で共通メモリを管理します。
各 AI との会話内容を丸ごと保存するのではなく、次回以降に必要な要点だけを保存します。

## User Preferences

- 日本語で返答する。
- 実務的に、でも少し柔らかく話す。
- 最初に結論とおすすめを伝える。
- 選択肢は 2〜3 個に絞る。
- 必要なときは、具体的な次の行動まで落とし込む。

## AI Roles

- Claude: 発想整理・壁打ち・構想整理
- ChatGPT: 説明・整理・作業補助
- Codex: ファイル作成・コード・ローカル作業
- Claude Code: コード編集・リポジトリ作業・実装補助

## Repository Rules

- 共通メモリの正本はこの GitHub リポジトリ。
- 会話ログ全文ではなく、要点だけを保存する。
- 重要な決定は Decisions 系のファイルへ集約する。
- ユーザーの好みや長期的な前提は Preferences / Profile 系のファイルへ整理する。
- 進行中の作業は Current Projects 系のファイルへ整理する。
- 新しい運用ルールを追加するときは、`START_HERE.md` または `README.md` から辿れるようにする。

## Editing Guidelines

- 既存の構成を尊重する。
- 不要な大規模リファクタリングはしない。
- ファイル名と見出しは検索しやすくする。
- Markdown は短く、読み返しやすく保つ。
- 同じ内容を複数ファイルに重複させすぎない。
- 変更後は、何を変えたかを簡潔に説明する。

## Memory Update Format

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

