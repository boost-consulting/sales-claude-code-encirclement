# Sales Claude Code Encirclement

Claude Codeで「無敗営業」フレームワークに基づいた営業アドバイスを得るための設定ファイル集。

## 概要

営業案件について相談すると、以下のフレームワークに基づいた具体的なアクション・質問・反応を提案します:

- **案件の3分類**: 楽勝 / 接戦 / 惨敗
- **接戦の3パターン**: コンペ / 先延ばし / 内製検討
- **接戦を制する3つの質問**: 接戦状況 / 決定の場面 / 裏の背景
- **BANTCHフレームワーク**: Budget / Authority / Needs / Timing / Competitor / Human

## 使い方

### 1. プロジェクトをクローン

```bash
git clone https://github.com/boost-consulting/sales-claude-code-encirclement.git
cd sales-claude-code-encirclement
```

### 2. Claude Codeで営業相談

プロジェクト内でClaude Codeを起動し、営業の悩みを相談:

```
claude
> 競合とのコンペで迷っている案件がある。どうすればいい？
```

### 3. /sales-advice コマンド（オプション）

対話形式で状況を分析したい場合は、`sales-advice.md` を `~/.claude/commands/` にコピー:

```bash
cp docs/sales-advice.md ~/.claude/commands/
```

その後、Claude Codeで `/sales-advice` を実行。

## ファイル構成

```
.
├── CLAUDE.md                          # プロジェクト設定（クイックスタート）
├── README.md                          # このファイル
├── docs/
│   └── sales-advice.md                # /sales-advice コマンド
└── .claude/
    └── rules/
        ├── sales-action-guide.md      # 営業アクションガイド
        └── questioning-techniques.md  # 質問テクニック詳細
```

## 質問例

| 相談内容 | 得られるアドバイス |
|---------|-------------------|
| 競合に負けそう | 差別化ポイントの訴求方法、使える質問 |
| お客さんが先延ばしにする | 今やらないリスクの提示方法 |
| 値引きを求められた | 安易に値引きしない対応パターン |
| 失注した理由を知りたい | 「決定の場面を問う質問」の使い方 |
| 案件の優先順位がわからない | 楽勝/接戦/惨敗の分類方法 |

## 参考書籍

- 高橋浩一『無敗営業』

## ライセンス

MIT
