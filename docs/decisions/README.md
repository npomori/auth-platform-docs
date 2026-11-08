# Architecture Decision Records (ADR)

設計上重要な決定と、その背景・選択肢・影響を記録します。

## ADRの作成ルール

- 重要なアーキテクチャ判断ごとに1ファイル作成する。
- ファイル名は `NNNN-short-title.md` とする。
- 状態は Proposed / Accepted / Superseded / Deprecated 等で管理する。
- 決定を変更した場合は、過去のADRを消さず、新しいADRから参照する。

## テンプレート

```markdown
# ADR NNNN: タイトル

- Status: Proposed
- Date: YYYY-MM-DD

## Context
背景・解決したい課題。

## Decision
採用する方針。

## Alternatives
検討した代替案と採用しなかった理由。

## Consequences
メリット、デメリット、移行・運用への影響。
```
