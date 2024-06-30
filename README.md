# ETHIntermediateModule3
# AshiErc20 Token

AshiErc20 is an ERC20 token smart contract built on the Ethereum blockchain. It implements a custom token named "Tikku" with the symbol "TK".

## Features

- ERC20 compliant
- Minting capability (restricted to owner)
- Burning capability
- Custom transfer function

## Contract Details

- Name: Tikku
- Symbol: TK
- Decimals: 18 (standard ERC20)

## Functions

### Constructor

- Initializes the token with a name, symbol, and initial supply
- Sets the contract deployer as the admin

### mint

- Allows the admin to mint new tokens to a specified address

### burn

- Allows any token holder to burn their own tokens

### transferAmount

- A custom transfer function that handles decimal conversion

## Usage

1. Deploy the contract, specifying the initial supply
2. Use standard ERC20 functions for transfers and allowances
3. Admin can mint new tokens using the `mint` function
4. Token holders can burn their tokens using the `burn` function
5. Use `transferAmount` for simplified token transfers

## Security

- The `onlyOwner` modifier restricts certain functions to the admin
- Built on OpenZeppelin's battle-tested ERC20 implementation

## License

This project is licensed under the MIT License.

## Dependencies

- OpenZeppelin Contracts v4.0.0
