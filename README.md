# Ethereum_Beginner

# MyToken

It is a simple Solidity contract represents a token. This contract gives tools like minting and burning tokens, and also storing token details such as name, abbreviation and total supply. 

## Contract Details

The contract includes the following public variables:

- `tokenName`: A string variable that represents the name of the token.
- `tokenAbbrv`: A string variable that represents the abbreviation or symbol of the token.
- `totalSupply`: An unsigned integer variable that stores the total supply of tokens.

And, also this contract having a mapping of addresses to balances:

- `balances`: It is a mapping that conects addresses with their related token balances.

## Functions

The contract provides the following functions:

### `mint`

The 'mint' function is used to create new tokens and allocate them to a specified address. It takes two parameters:

- 'address': The Ethereum address to which the newly minted tokens will be allocated.
- 'value': The number of tokens to be minted.

The function increases the total supply by the specified 'value' and adds the minted tokens to the balance of the designated address.

### `burn`

The 'burn' function allows for the destruction of tokens. It works in the opposite way to the 'mint' function. It takes two parameters:

- 'address': The Ethereum address from which the tokens will be burned.
- 'value': The number of tokens to be burned.

The function checks if the balance of the designated address is greater than or equal to the specified 'value'. If the condition is met, it decreases the total supply and deducts the specified amount from the address's balance.

## License

This project is licensed under the Solidity Assessment License - see the [License.md](LICENSE.md) file for details

## Authors

- Harshit Kumar
