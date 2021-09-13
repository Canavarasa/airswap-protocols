<br />
<img src="https://www.airswap.io/airswap-blue-transparent.png" width="500"/>
<br />

[AirSwap](https://www.airswap.io/) is a peer-to-peer trading network for Ethereum tokens, initially built on the [Swap Protocol](https://www.airswap.io/whitepaper.htm). This repository contains smart contracts and JavaScript packages for use by developers and traders on the AirSwap network.

[![Discord](https://img.shields.io/discord/590643190281928738.svg)](https://chat.airswap.io)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/MIT)
[![lerna](https://img.shields.io/badge/maintained%20with-lerna-cc00ff.svg)](https://lerna.js.org/)
![Twitter Follow](https://img.shields.io/twitter/follow/airswap?style=social)

## Resources

- About → https://about.airswap.io/
- Website → https://www.airswap.io/
- Twitter → https://twitter.com/airswap
- Chat → https://chat.airswap.io/

## Smart Contracts

Packages are versioned based on deploys. Major versions e.g. `1.x.x` are mainnet deploys, while minor versions e.g. `x.1.x` are rinkeby deploys. Packages that are not deployed increment patch versions e.g. `x.x.1`. Each package that includes a deployment includes the ABI files for that deployed contract in `build/contracts` within the package.

| Package                                 | Version                                                                                                   | Description                    |
| :-------------------------------------- | :-------------------------------------------------------------------------------------------------------- | :----------------------------- |
| [`@airswap/light`](/source/light)       | [![npm](https://img.shields.io/npm/v/@airswap/light)](https://www.npmjs.com/package/@airswap/light)       | Atomic Swap Between Tokens     |
| [`@airswap/registry`](/source/registry) | [![npm](https://img.shields.io/npm/v/@airswap/registry)](https://www.npmjs.com/package/@airswap/registry) | Counterparty Discovery         |
| [`@airswap/staking`](/source/staking)   | [![npm](https://img.shields.io/npm/v/@airswap/staking)](https://www.npmjs.com/package/@airswap/staking)   | Staking for Participation      |
| [`@airswap/pool`](/source/pool)         | [![npm](https://img.shields.io/npm/v/@airswap/pool)](https://www.npmjs.com/package/@airswap/pool)         | Rewards Pool for Participation |

## JavaScript Libraries

| Package                                  | Version                                                                                                     | Description           |
| :--------------------------------------- | :---------------------------------------------------------------------------------------------------------- | :-------------------- |
| [`@airswap/protocols`](/tools/protocols) | [![npm](https://img.shields.io/npm/v/@airswap/protocols)](https://www.npmjs.com/package/@airswap/protocols) | Protocol Clients      |
| [`@airswap/utils`](/tools/utils)         | [![npm](https://img.shields.io/npm/v/@airswap/utils)](https://www.npmjs.com/package/@airswap/utils)         | Orders and Signatures |
| [`@airswap/metadata`](/tools/metadata)   | [![npm](https://img.shields.io/npm/v/@airswap/metadata)](https://www.npmjs.com/package/@airswap/metadata)   | Metadata Management   |
| [`@airswap/constants`](/tools/constants) | [![npm](https://img.shields.io/npm/v/@airswap/constants)](https://www.npmjs.com/package/@airswap/constants) | Helpful Constants     |

## Commands

| Command        | Description                                                                   |
| :------------- | :---------------------------------------------------------------------------- |
| `yarn compile` | Compile all contracts to `build` folders.                                     |
| `yarn clean`   | Delete all contract `build` folders.                                          |
| `yarn ganache` | Run a local `ganache` network on local host 8545.                             |
| `yarn test`    | Run all contract tests in `test` folders. Run `yarn ganache` elsewhere first. |
| `yarn hint`    | Run a syntax linter for all Solidity code.                                    |
| `yarn lint`    | Run a syntax linter for all JavaScript code.                                  |
| `yarn deps`    | Run a dependency consistency check.                                           |

## Deployments

To deploy, please follow [this guide](./tools/deployer)
