# MyToken Solidity Smart Contract

This is a simple Solidity smart contract for an ERC-20 like token named `META` with the abbreviation `MTA`. The contract allows minting and burning of tokens, and keeps track of balances and total supply  for different addresses.

## Contract Details

- **Token Name**: META
- **Token Abbreviation**: MTA
- **Total Supply**: The total supply of the token, initially set to 0 and can be increased by minting.

## Public Variables

- `string public tokenName = "META";`
- `string public tokenAbbrv = "MTA";`
- `uint public totalsupply = 0;`

## Mapping

- `mapping(address => uint) public balances;` - A mapping to keep track of the balance of each address.

## Functions

### Mint

This function mints new tokens and assigns them to a specified address. It increases both the total supply and the balance of the given address.

## Burn 

This function destroys tokens that have been  minted . Condition has been put on burn function if the value put inside it is larger than the total supply and balnce , then it will  not work .
