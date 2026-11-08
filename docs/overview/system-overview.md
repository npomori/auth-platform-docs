# System Overview

## 1. 目的

複数の独立したWebアプリケーションが、共通の認証サーバーを利用してユーザー認証とユーザー基盤を共有できるようにする。

## 2. 構成要素

| コンポーネント | リポジトリ | 主な責任 |
|---|---|---|
| 認証サーバー | [auth-server](https://github.com/npomori/auth-server) | 認証、ユーザー管理、共通ロール、参加アプリ管理 |
| 参加アプリ共通基盤 | [participant-app-base](https://github.com/npomori/participant-app-base) | 認証サーバーとの連携、参加アプリ共通処理 |
| サンプル参加アプリ | [sample-app](https://github.com/npomori/sample-app) | 参加アプリの実装例・動作確認 |

## 3. 基本的な考え方

- 認証サーバーは、システム共通のユーザー認証とユーザー基盤を管理する。
- 参加アプリは、認証サーバーと連携して認証済みユーザーを利用する。
- 参加アプリは、アプリ固有の業務機能や権限を管理する。
- 新しい参加アプリは、共通基盤と連携仕様に従って追加する。

## 4. 利用者・権限の概要

共通ロールと参加アプリ固有ロールを区別する。具体的な割り当て・変更規則は [Roles and Permissions](../specification/roles-and-permissions.md) を参照。

## 5. 関連資料

- [Architecture](architecture.md)
- [Components](components.md)
- [Authentication](../specification/authentication.md)
- [Participant App Guide](../integration/participant-app-guide.md)

## 6. 確認・確定が必要な事項

- 本番環境における各アプリの配置・ネットワーク構成
- 認証連携プロトコルとトークン／コードの仕様
- ユーザー情報・アプリ情報のデータ共有範囲
- ログアウト時の全アプリへの影響範囲
