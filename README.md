# swiftTech884

このリポジトリは [Obsidian](https://obsidian.md/) の Vault として利用でき、
[Claudian](https://github.com/YishenTu/claudian)（Claude Code などのコーディングエージェントを Obsidian に組み込むプラグイン）を導入済みです。

## 導入内容

| パス | 内容 |
| --- | --- |
| `.obsidian/plugins/realclaudian/` | Claudian v2.3.20 の公式リリースファイル（`main.js` / `manifest.json` / `styles.css`） |
| `.obsidian/community-plugins.json` | Claudian を有効化する設定 |

## 必要環境

- Obsidian v1.13.0 以降（デスクトップ版のみ：macOS / Linux / Windows）
- [Claude Code](https://docs.claude.com/en/docs/claude-code) CLI がインストール・ログイン済みであること
  （Codex、OpenCode など他の対応エージェントでも可）

## セットアップ手順

1. このリポジトリをクローンする
   ```bash
   git clone https://github.com/swiftTech884/swiftTech884.git
   ```
2. Obsidian で「フォルダを保管庫として開く」からクローンしたフォルダを開く
3. 「制限モード」を求められたら **コミュニティプラグインを有効化** を選ぶ
4. 設定 → コミュニティプラグイン で **Claudian** がオンになっていることを確認
5. サイドバーの Claudian アイコンからチャットを開始

## トラブルシューティング

- **CLI が見つからない**: 設定 → Claudian → Providers → Claude Code で CLI のパスを指定
- **Node.js が別ディレクトリにある**: 設定 → Claudian → General → Environment に `PATH=/path/to/node/bin` を追加
- **サブスクリプションで認証できない**: Providers → Claude Code → Environment → Custom variables に `ANTHROPIC_API_KEY=`（空値）を追加

## アップデート

Obsidian の 設定 → コミュニティプラグイン → 「アップデートを確認」から更新できます。
