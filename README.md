#  MyToken Smart Contract

## Overview
This Solidity smart contract implements a basic token functionality with minting and burning capabilities. It allows for the creation, distribution, and destruction of tokens.

## Requirements
1. The contract includes public variables to store the details about the coin (Token Name, Token Abbreviation, Total Supply).
2. It features a mapping of addresses to balances (`address => uint`), representing the token balances of individual addresses.
3. A mint function is provided that increases the total supply by a specified amount and increments the balance of a given address.
4. The contract also includes a burn function, which decreases the total supply and deducts tokens from the balance of a specified address.
5. The burn function includes conditionals to ensure that the balance of the address is sufficient for the intended burn amount.

#   Implementation Details
###  Public Variables
- `Token_name`: Stores the name of the token.
- `Token_abb`: Stores the abbreviation of the token.
- `Total_supply`: Stores the total supply of the token.

###  Mapping
- `map`: Maps addresses to their corresponding token balances.

###  Mint Function
- `mint(address _a, uint _y)`: Increases the total supply by the specified amount `_y` and adds the same amount to the balance of the address `_a`.

###  Burn Function
- `burn(address _a, uint _y)`: Checks if the balance of the address `_a` is greater than or equal to the specified burn amount `_y`. If so, it reduces the total supply by `_y` and deducts the same amount from the balance of `_a`.

## Usage
1. Deploy the `MyToken` contract on a compatible Ethereum Virtual Machine (EVM) such as Ethereum or any EVM-compatible blockchain.
2. Interact with the contract by calling its `mint` and `burn` functions to create and destroy tokens, respectively.
3. Ensure proper permissions and authentication mechanisms are in place for accessing the mint and burn functions.

## License
This smart contract is licensed under the MIT License. See the `LICENSE` file for more details.

## Author 
Saurabh Kumar

 
