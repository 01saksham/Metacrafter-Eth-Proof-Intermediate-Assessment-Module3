# Ember Token (EMB)

The Ember Token (EMB) is an ERC20-compliant token built on the Ethereum blockchain. It provides a basic set of functionalities for transferring, minting, and burning tokens.

## Contract Details

- Token Name: Ember Token
- Token Symbol: EMB
- Decimals: 18

## Functions

### `transfer`

```solidity
function transfer(address recipient, uint amount) external returns (bool);
```

This function allows the caller to transfer a specified amount of tokens from their own account to the recipient's account. The caller must have a sufficient balance to execute the transfer.

### `mint`

```solidity
function mint(uint amount) external onlyOwner;
```

The `mint` function enables the contract owner to create new tokens and add them to their own account. Only the contract owner can call this function.

### `burn`

```solidity
function burn(uint amount) external;
```

The `burn` function allows an account to burn a specified amount of tokens, effectively reducing the total supply. The caller must have a sufficient balance to execute the burn.

### `totalSupply`

```solidity
function totalSupply() external view returns (uint);
```

The `totalSupply` function returns the total number of tokens in circulation.

### `balanceOf`

```solidity
function balanceOf(address account) external view returns (uint);
```

The `balanceOf` function retrieves the token balance of the specified account.

## License

This contract is released under the MIT License. You can find more details in the [LICENSE](LICENSE) file.

Feel free to update this README file with any additional information about your specific implementation, usage instructions, or project details.
