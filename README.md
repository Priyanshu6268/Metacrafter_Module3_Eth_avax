
# Metacrafter Types of Function ETH+AVAX Course Project

## Overview

This repository contains a Solidity smart contract for an ERC20 token, created as part of the third module of the ETH+AVAX course. The smart contract allows for the minting, burning, and transferring of tokens.

## Requirements

- A GitHub account and a public repository to share your project.
- A README file to provide an overview of your project (You're reading it!).
- A video walkthrough explaining the codebase (Link to be added).
- This project does not require sharing a transaction ID.

## Features

1. **Minting Tokens**: The contract owner can mint new tokens to a provided address.
2. **Burning Tokens**: Any user can burn their tokens, reducing the total supply.
3. **Transferring Tokens**: Tokens can be transferred from one address to another.

## Prerequisites

- Solidity ^0.8.0
- HardHat or Remix for deployment
- ERC20 from OpenZeppelin as a dependency

## Installation

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/metacrafter-eth-avax.git
   ```
2. Install dependencies
   ```bash
   npm install
   ```

## Deployment

1. Compile the contract
   ```bash
   npx hardhat compile
   ```
2. Deploy the contract
   ```bash
   npx hardhat run scripts/deploy.js --network localhost
   ```

## Usage

1. **Mint Tokens**
   ```solidity
   function mint(address to, uint256 amount) public onlyOwner
   ```
2. **Burn Tokens**
   ```solidity
   function burn(uint256 amount) public
   ```
3. **Transfer Tokens**
   ```solidity
   function transfer(address recipient, uint256 amount) public returns (bool)
   ```

## Video Walkthrough

[[https://www.loom.com/share/3b98079def6840619d7a3a30adeb3daa]](#) (Link to be added)

## Further Information

In the video, I provide a code walkthrough where I discuss:
- The main function and its purpose
- The transfer function and how it operates
- The deployment process, including the use of HardHat/Remix
- The Solidity version used and the OpenZeppelin ERC20 import
- A live demonstration of deploying, minting, burning, and transferring tokens

## License

MIT License
