# SaveEther

A simple Solidity smart contract for saving Ether and ERC20 tokens.

## Overview

SaveERC20andEther is a savings contract that allows users to deposit and withdraw both native Ether and ERC20 tokens. Each user's savings are tracked separately and can be withdrawn at any time.

## Features

- **Deposit Ether**: Save native Ether to the contract
- **Withdraw Ether**: Withdraw your saved Ether
- **Deposit ERC20 Tokens**: Save any ERC20 token to the contract
- **Withdraw ERC20 Tokens**: Withdraw your saved tokens
- **Check Balances**: View your Ether and token savings

## Contract Functions

### Ether Functions
- `depositEther()` - Deposit Ether to your savings
- `withdrawEther(uint256 amount)` - Withdraw Ether from your savings
- `getEtherBalance(address user)` - Check Ether balance for a user

### Token Functions
- `depositToken(address token, uint256 amount)` - Deposit ERC20 tokens (requires approval)
- `withdrawToken(address token, uint256 amount)` - Withdraw ERC20 tokens
- `getTokenBalance(address user, address token)` - Check token balance for a user

## Requirements

- Solidity ^0.8.20
- Users must approve the contract to spend their ERC20 tokens before depositing

## License

MIT
