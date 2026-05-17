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

## 2026-05-18

- ChatGPT から GitHub リポジトリ `zosuntowa-a11y/ai-memory` への書き込み権限を確認した。
- ChatGPT は `main` に直接 push せず、原則として更新用ブランチを作成し、Pull Request で共通メモリの変更提案を出す。
- 共通メモリ更新は、完全自動ではなく「会話から重要事項を抽出 → 更新案を作成 → 必要に応じてPR化 → 人間またはClaude Codeが確認して反映」の半自動フローにする。
- 保存対象は、今後も使う前提・決定事項・好みや方針・継続中プロジェクトに絞る。
- `main` ブランチにブランチ保護（Pull Request 必須）を設定した。ChatGPT/Codex（非管理者の GitHub App）は `main` 直 push がブロックされ、PR 経由のみになる。管理者は保護をバイパス可能。
- この Mac から GitHub への push は SSH 鍵方式に統一した（HTTPS のパスワード/トークン認証は GitHub 側で廃止済みのため）。
- PR をマージした後は、ローカル `/Users/satotowa/ai-memory` で `git pull` して正本（Google Drive 同期フォルダ）へ反映する。GitHub 上でのマージだけでは正本は更新されない。
- 共通メモリは「貯める（会話の節目で更新案→PR）」だけでなく「整理する（月1回ほど重複統合・古い情報の削除）」を習慣にする。貯めるだけだと量が増えるほど使いにくくなるため。
