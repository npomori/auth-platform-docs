# Authentication Platform

複数のWebアプリケーションで認証基盤を共有するための統合認証プラットフォームです。

## System Architecture

本システムは、認証サーバーを中心に、複数の参加アプリケーションで構成されます。

| Repository | Role |
|---|---|
| [auth-server](https://github.com/npomori/auth-server) | 認証、ユーザー管理、共通ロール、参加アプリ管理 |
| [participant-app-base](https://github.com/npomori/participant-app-base) | 参加アプリ向け共通基盤、認証連携、アクセス制御 |
| [sample-app](https://github.com/npomori/sample-app) | 参加アプリの実装例 |

## Documentation

### Overview
- [System Overview](docs/overview/system-overview.md)
- [Architecture](docs/overview/architecture.md)
- [Components](docs/overview/components.md)

### Specifications
- [Authentication](docs/specification/authentication.md)
- [Session Management](docs/specification/session-management.md)
- [App Integration](docs/specification/app-integration.md)
- [User Management](docs/specification/user-management.md)
- [Roles and Permissions](docs/specification/roles-and-permissions.md)
- [Data Sharing](docs/specification/data-sharing.md)

### Integration
- [App Registration](docs/integration/app-registration.md)
- [Participant App Guide](docs/integration/participant-app-guide.md)
- [Integration Flow](docs/integration/integration-flow.md)

### Operation
- [Deployment](docs/operation/deployment.md)
- [Environment](docs/operation/environment.md)
- [Security](docs/operation/security.md)
- [Troubleshooting](docs/operation/troubleshooting.md)

### Decisions
- [Architecture Decision Records](docs/decisions/README.md)

## Related Repositories

- https://github.com/npomori/auth-server
- https://github.com/npomori/participant-app-base
- https://github.com/npomori/sample-app

## Documentation Ownership

- システム全体の共通仕様・アプリ間の契約は、このリポジトリを正本とします。
- 各アプリ内部の実装詳細は、それぞれのアプリのリポジトリを正本とします。
- 同じ仕様を複数のリポジトリに重複して記載せず、必要に応じて相互リンクします。
- 共通仕様を変更した場合は、関連する各リポジトリへの影響と実装状況を確認します。

## Status

このリポジトリは統合ドキュメントの初期構成です。各仕様の詳細は、実装・既存資料との照合を行いながら確定してください。
