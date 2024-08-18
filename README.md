# swisstronik-perc-20

This repository contains a setup for deploying and interacting with an PERC-20 token on the Swisstronik testnet using Hardhat. The setup includes scripts for deploying the contract, minting tokens, and transferring tokens, utilizing encrypted transactions with Swisstronik.

## Prerequisites

Ensure you have the following installed:

- Node.js (version 14.x or later)
- npm (version 6.x or later)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/web3bustler/swisstronik-perc-20.git
    cd swisstronik-perc-20
    ```

2. Make the `perc20.sh` script executable:

    ```bash
    chmod +x perc20.sh
    ```

## Usage

1. Run the script:

    ```bash
    ./perc20.sh
    ```

2. Follow the prompts to enter your private key and specify the token name and symbol.

## Scripts

### `deploy.js`

This script deploys the PERC-20 contract and saves the deployed contract address to `contract.txt`.

### `mint.js`

This script mints 100 tokens using the deployed contract. It reads the contract address from `contract.txt`.

### `transfer.js`

This script transfers tokens from the contract to a specified address. It reads the contract address from `contract.txt`.

## Notes

- Ensure your private key is kept secure.
- The `transfer.js` script is set to transfer tokens to the address `0x16af037878a6cAce2Ea29d39A3757aC2F6F7aac1` with an amount of `1 * 10 ** 18` tokens. Modify these values as needed.
