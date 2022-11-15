# USE CARDANO

## Unreleased 

**OBS!! This project is unreleased. Feel free to use it, but be aware that it is to be considered as an alpha version. Things can break, the APIs will change etc.**

## At a glance

`use-cardano` is a react hook that makes interacting with the Cardano blockchain easy. The library lets you connect web3 dapp wallets using the CIP-30 Web Bridge and [lucid-cardano](). It is written in TypeScript and uses the aforementioned library lucid-cardano for functionality such as signing transactions and more.

## Usage

1. Install the package `npm install use-cardano`
1. Install the package's peerDependencies `npm i lucid-cardano react`
1. Import the hook `import { useCardano } from 'use-cardano'`
1. Set your blockfrost env variables in your `.env` file (see `/example/.env.template`)
1. Use the hook

_I am looking to add support for more providers besides blockfrost as lucid-cardano does the same._

## Examples

See the `/example` folder

## Contributing / Development

Feel free to contribute in any capacity you can and want to. Either by opening an issue, creating a pull request or just by giving feedback.

### Running the project in development mode

1. Clone the repository
1. Install pnpm: `npm i -g pnpm` (this is recommended over npm or yarn because it handles dependency linking better)
1. Install example dependencies: `cd example && pnpm i && cd ..`
1. Link the library run time dependencies: `pnpm link ./example/node_modules/react ./example/node_modules/lucid-cardano`
1. Install library dependencies: `pnpm i`
1. Run the library in watch mode, and launch the example app: `pnpm run dev`

### Example app

There is an example app in the `/example` folder. It is a simple react app that uses the library. It is set up to use the library in development mode, so you can make changes to the library and see the changes in the example app.

![Example app](.github/example-app.png)