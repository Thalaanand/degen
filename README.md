# Degen Token

## Overview

This repository contains the source code for a decentralized laptop subscription smart contract built on the Ethereum blockchain. The smart contract, named "LaptopSubscription," is an ERC-20 token (Degen - DGN) that allows users to redeem different laptop models by spending a specific amount of tokens. The contract also includes functionality for minting, burning tokens, and modifying the user's laptop model.

## Smart Contract Features

### ERC-20 Token

- The smart contract implements the ERC-20 standard, providing basic token functionality such as transfer, approval, and balance checking.

### Laptop Models

- The contract defines four laptop models: HP, DELL, MAC, and ASUS, each associated with a specific cost in tokens.

### Subscription Redemption

- Users can redeem a laptop by specifying the model number (1 to 4) they wish to acquire.
- The smart contract verifies the user's balance, burns the required tokens, and updates the user's laptop subscription.

### Minting Tokens

- The owner of the smart contract can mint new tokens and distribute them to specified addresses.

### Burning Tokens

- Users can burn a specific amount of their own tokens, reducing their token balance.

### Modifying Laptop Model

- Users can modify their laptop subscription by selecting a new laptop model. The smart contract updates the user's subscription accordingly.

## Events

The smart contract emits several events to provide transparency and allow easy tracking of important activities:

1. `SubscriptionRedeemed`: Triggered when a user redeems a laptop subscription, indicating the account, laptop model, and subscription cost.
2. `TokensBurned`: Fired when a user burns a certain amount of tokens, providing information about the account and the burned amount.
3. `LaptopModelModified`: Indicates when a user modifies their laptop model, revealing the updated model and the associated account.

## Constants

The smart contract includes predefined costs for each laptop model:

- HP: 150 Degen tokens
- DELL: 180 Degen tokens
- MAC: 250 Degen tokens
- ASUS: 200 Degen tokens

## Getting Started

1. Deploy the smart contract to an Ethereum network.
2. Mint some Degen tokens to distribute or allocate to users.
3. Users can interact with the contract to redeem laptops, burn tokens, and modify their laptop models.

## Development Environment

- Solidity version: 0.8.18
- Dependencies: OpenZeppelin contracts for ERC-20 and Ownable functionalities.

## License

This smart contract is released under the MIT License. See the `LICENSE` file for details.

