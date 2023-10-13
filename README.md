# Module21Challenge
# KaseiCoin Crowdsale Project

## Project Description

The KaseiCoin Crowdsale Project is a blockchain-based initiative aimed at launching a new cryptocurrency called KaseiCoin (KAI) for the burgeoning Martian colony. Leveraging the Ethereum blockchain, this project establishes a monetary system by minting and distributing KaseiCoin tokens through a crowdsale. The project comprises three main smart contracts:

1. **KaseiCoin (KAI) Token Contract:** Defines KaseiCoin as an ERC-20 compliant token.
2. **KaseiCoin Crowdsale Contract:** Manages the crowdsale process, allowing participants to exchange Ether for KaseiCoin.
3. **KaseiCoin Crowdsale Deployer Contract:** Orchestrates the deployment of the above two contracts.

## Dependencies

- [Remix IDE](https://remix.ethereum.org/)
- [OpenZeppelin Contracts v2.5.0](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag/v2.5.0)
- [MetaMask](https://metamask.io/)
- [Ganache](https://www.trufflesuite.com/ganache)

## Setup and Deployment

### Step 1: Smart Contract Development

- Create and compile the smart contracts (`KaseiCoin.sol` and `KaseiCoinCrowdsale.sol`) using Remix IDE.
- Using Version 5.5.0
  
### Step 2: Local Blockchain Setup

- Run Ganache to initiate a local blockchain.
- Configure MetaMask to connect to your local blockchain.
- Import wallet seed phase from Ganache into MetaMask

### Step 3: Contract Deployment

- In Remix, navigate to the "Deploy & Run Transactions" tab.
- Select the appropriate environment (Injected Web3 for Metamask).
- Deploy `KaseiCoinCrowdsaleDeployer` with the necessary constructor arguments (name, symbol, wallet address).

### Step 4: Interacting with the Contracts

- After deployment, the addresses of the deployed `KaseiCoin` and `KaseiCoinCrowdsale` contracts can be found in the transaction details.
- Use MetaMask to interact with the contracts.
- To purchase KaseiCoin, send Ether to the `KaseiCoinCrowdsale` contract address. (default ratio is 1 ETH = 1 KSC)

## Testing

Test the functionality of the crowdsale using different accounts to buy tokens, check balances, and ensure the crowdsale processes transactions as expected.

## Screenshots

![Token Creation](Screenshot/1.Token%20Creation.jpg)
![Token Creation Hash](Screenshot/2.Token%20Creation%20Hash.jpg)
![Token Creation Block](Screenshot/3.Token%20Creation%20Blockjpg)
![Token Deployer](Screenshot/4.Token%20Deployer.jpg)
![Token Deployer Hash](Screenshot/5.Token%20Deployer%20Hash.jpg)
![Token Deployer Transaction](Screenshot/6.Token%20Deployer%20Transaction.jpg)
![Test Buying Metamask](Screenshot/7.Test%20Buying%20Metamask.jpg)
![Test Buying Transaction](Screenshot/8.Test%20Buying%20Transtion.jpg)