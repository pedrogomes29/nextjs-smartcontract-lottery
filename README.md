# FundMe FrontEnd

&nbsp;&nbsp; This repository holds the user interface to interact with the [Decentralized Lottery](https://github.com/pedrogomes29/decentralized-lottery)

&nbsp;&nbsp; This smart contract runs on the [Rinkeby network](https://www.rinkeby.io/) (please don't spam it as it is a non-profit test network). Get some ETH from a faucet.
- Main Faucet: https://faucets.chain.link
- Backup Faucet: https://rinkebyfaucet.com/

&nbsp;&nbsp; In this UI you can connect your wallet to the website and join the lottery. A winner (assuming at least one person joined) is chosen randomly (using [Chainlink VRF](https://vrf.chain.link/)) every 30 seconds (using [Chainlink Keepers](https://keepers.chain.link/))

# Getting Started

## Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [Nodejs](https://nodejs.org/en/)
  - You'll know you've installed nodejs right if you can run:
    - `node --version` and get an ouput like: `vx.x.x`
- [Yarn](https://yarnpkg.com/getting-started/install) instead of `npm`
  - You'll know you've installed yarn right if you can run:
    - `yarn --version` and get an output like: `x.x.x`
    - You might need to [install it with `npm`](https://classic.yarnpkg.com/lang/en/docs/install/) or `corepack`

## Quickstart

```
git clone https://github.com/pedrogomes29/nextjs-smartcontract-lottery
cd nextjs-smartcontract-lottery
yarn
yarn dev
```


# Usage

1. Run your local blockchain with the lottery code

> In a different terminal / command line

```
git clone https://github.com/pedrogomes29/decentralized-lottery
cd decentralized-lottery
yarn 
yarn hardhat node
```


2. Add hardhat network to your metamask/wallet

- Get the RPC_URL of your hh node (usually `http://127.0.0.1:8545/`)
- Go to your wallet and add a new network. [See instructions here.](https://metamask.zendesk.com/hc/en-us/articles/360043227612-How-to-add-a-custom-network-RPC)
  - Network Name: Hardhat-Localhost
  - New RPC URL: http://127.0.0.1:8545/
  - Chain ID: 31337
  - Currency Symbol: ETH (or GO)
  - Block Explorer URL: None

Ideally, you'd then [import one of the accounts](https://metamask.zendesk.com/hc/en-us/articles/360015489331-How-to-import-an-Account) from hardhat to your wallet/metamask. 

3. Run this code

Back in a different terminal with the code from this repo, run:

```
yarn dev
```

4. Go to the UI and have fun!

Head over to your [localhost](http://localhost:3000) and play with the lottery!


5. Simulate Chainlink Keepers and VRF

Run a script which mocks Chainlink Keepers and Chainlink VRF

```
yarn run mockOffchain
```

## License
[MIT](https://choosealicense.com/licenses/mit/)

