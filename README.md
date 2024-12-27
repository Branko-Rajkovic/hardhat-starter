# hardhat-starter

A simple smart contract that implements a token that can be transferred.

-There is a fixed total supply of tokens that can't be changed.
-The entire supply is assigned to the address that deploys the contract.
-Anyone can receive tokens.
-Anyone with at least one token can transfer tokens.
-The token is non-divisible. You can transfer 1, 2, 3, or 37 tokens but not 2.5.

To compile the contract run in your terminal:
npx hardhat compile

# Testing contracts

To test the contract, we are going to use Hardhat Network, a local Ethereum network designed for development.
It comes built-in with Hardhat, and it's used as the default network. You don't need to setup anything to use it.
In your terminal run:
npx hardhat test

# Deploying contract

To deploy to Hardhat network run in terminal:
npx hardhat ignition deploy ./ignition/modules/Token.js

To deploy to Sepolia network run in terminal:
npx hardhat ignition deploy ./ignition/modules/Token.js --network sepolia
