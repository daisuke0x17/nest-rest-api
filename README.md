## NestJS
- Node.jsのバックエンド開発フレームワーク
- Expressがベース
  - fastifyに切替可能
- Angularのソフトウェアアーキテクチャを導入
  - 可読性、保守性に優れたソフトウェア開発
- Expressのノウハウを活用しつつ高品質なソフトウェア開発が可能

## Memo
- DI (Dependency Injection)
  - ソフトウェアを疎結合にするためのデザインパターン
  - NestではControllerがServiceのメソッドを呼ぶことで処理を実行
  - Controller側でServiceをインスタンス化せずに利用できることが特徴！
    - ControllerのコンストラクタにServiceを引数で渡すと自動でインスタンス化
  - Moduleでcontrollerとproviders(service)を設定する必要がある

- Nestでの典型的なDIパターン
  - 自作のServiceをProviderにインジェクションするパターン
  - 外部モジュールをProviderにインジェクションするパターン
    - 外部モジュール側でexportsするとインポート側のServiceで利用可能になる

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ yarn install
```

## Running the app

```bash
# development
$ yarn run start

# watch mode
$ yarn run start:dev

# production mode
$ yarn run start:prod
```

## Test

```bash
# unit tests
$ yarn run test

# e2e tests
$ yarn run test:e2e

# test coverage
$ yarn run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).
