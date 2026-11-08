# Environment Configuration

## 1. 目的

各アプリケーションの環境設定を一元的に把握する。

## 2. 設定管理ルール

- 環境変数名、用途、設定先、必須／任意を一覧化する。
- 実際の秘密値は記載しない。
- 開発・検証・本番で値を分離する。
- 設定変更時は関連アプリへの影響を確認する。

## 3. 設定一覧テンプレート

| Variable | Component | Required | Description | Secret |
|---|---|---:|---|---:|
| `AUTH_SERVER_URL` | participant app | Yes | 認証サーバーのURL | No |
| `APP_CLIENT_ID` | participant app | Yes | 参加アプリ識別子 | No |
| `APP_CLIENT_SECRET` | participant app | 要確認 | 実装仕様に応じた秘密情報 | Yes |

上記は記載例です。実際の変数名・必須条件は各リポジトリの実装と照合してください。
