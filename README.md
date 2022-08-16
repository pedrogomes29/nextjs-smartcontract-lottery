# FundMe FrontEnd

&nbsp;&nbsp; This repository holds the user interface to interact with the [Decentralized Lottery](https://github.com/pedrogomes29/decentralized-lottery)

&nbsp;&nbsp; This web3 website runs on the [Rinkeby network](https://www.rinkeby.io/) (please don't spam it as it is a non-profit test network). Get some ETH from a faucet.
- Main Faucet: https://faucets.chain.link
- Backup Faucet: https://rinkebyfaucet.com/

&nbsp;&nbsp; In this UI you can connect your wallet to the website and join the lottery. A winner (assuming at least one person joined) is chosen randomly (using [Chainlink VRF](https://vrf.chain.link/)) every 30 seconds (using [Chainlink Keepers](https://keepers.chain.link/))

## Usage

Just change directory until you are in the project directory and then,assuming 
you already have nodejs and yarn installed, run this command 
```
yarn
```
which will download the needed dependencies
<br>
<br>
Then run
```
yarn dev
```
which will start [a local server](http://localhost:3000/) in which you can use the website
<br>
## License
[MIT](https://choosealicense.com/licenses/mit/)

