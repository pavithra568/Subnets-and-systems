# ERC20 and Vault Contracts - README

## Overview

This repository contains two smart contracts: an ERC20 token contract and a Vault contract. The ERC20 contract follows the ERC20 standard for fungible tokens on the Ethereum blockchain, while the Vault contract allows for secure storage and management of these ERC20 tokens.

## ERC20 Contract

The ERC20 contract implements a standard ERC20 token with additional functionalities. The primary features include:

- **Standard ERC20 functions**: `transfer`, `approve`, `transferFrom`, `balanceOf`, `totalSupply`, and `allowance`.
- **Minting and Burning**: Functions to mint new tokens and burn existing ones.
- **Ownership**: Ownership functionality to manage administrative actions.

### ERC20 Functions

#### `name()`
Returns the name of the token.

#### `symbol()`
Returns the symbol of the token.

#### `decimals()`
Returns the number of decimals the token uses.

#### `totalSupply()`
Returns the total token supply.

#### `balanceOf(address account)`
Returns the account balance of another account with address `account`.

#### `transfer(address recipient, uint256 amount)`
Transfers `amount` tokens to `recipient`. Returns a boolean value indicating whether the operation succeeded.

#### `approve(address spender, uint256 amount)`
Sets `amount` as the allowance of `spender` over the caller’s tokens. Returns a boolean value indicating whether the operation succeeded.

#### `transferFrom(address sender, address recipient, uint256 amount)`
Moves `amount` tokens from `sender` to `recipient` using the allowance mechanism. Returns a boolean value indicating whether the operation succeeded.

#### `allowance(address owner, address spender)`
Returns the remaining number of tokens that `spender` will be allowed to spend on behalf of `owner`.

#### `mint(address account, uint256 amount)`
Mints `amount` tokens to the `account`.

#### `burn(uint256 amount)`
Burns `amount` tokens from the caller’s account.

## Vault Contract

The Vault contract allows users to deposit and withdraw ERC20 tokens securely. It provides functionalities to store tokens, check balances, and withdraw tokens.

### Vault Functions

#### `deposit(uint256 amount)`
Deposits `amount` tokens into the vault.

#### `withdraw(uint256 amount)`
Withdraws `amount` tokens from the vault.

#### `balanceOf(address account)`
Returns the balance of the specified `account` in the vault.


## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

