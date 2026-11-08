# Components

## auth-server

- Repository: https://github.com/npomori/auth-server
- 責任: 共通認証、ユーザー管理、共通ロール、参加アプリ管理
- 内部実装・API詳細: auth-server リポジトリの docs を正本とする

## participant-app-base

- Repository: https://github.com/npomori/participant-app-base
- 責任: 参加アプリ向けの共通連携機能・アクセス制御
- 内部実装・利用方法: participant-app-base リポジトリの docs を正本とする

## sample-app

- Repository: https://github.com/npomori/sample-app
- 責任: 参加アプリの実装例、統合動作の確認
- 個別機能の実装詳細: sample-app リポジトリの docs を正本とする

## Component Change Checklist

- [ ] 他コンポーネントとのインターフェースに変更があるか
- [ ] 共通仕様の更新が必要か
- [ ] 参加アプリ共通基盤への影響があるか
- [ ] 既存の参加アプリへの互換性を確認したか
- [ ] サンプルアプリ・テストを更新したか
