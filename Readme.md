## TOPG - Tokenized Ownership Proof Generator

TOPG is a Solidity smart contract that implements the ERC721 standard for non-fungible tokens (NFTs). It provides functionalities for minting, pausing, and managing ownership of NFTs.

### Features

- **ERC721 Compliance**: Implements the ERC721 standard for NFTs.
- **Enumerable and Pausable**: Extends ERC721 with enumerable and pausable functionalities.
- **Owner Management**: Includes functions for managing ownership and minting permissions.
- **IPFS Metadata**: Provides a base URI for IPFS metadata of the tokens.

### Prerequisites

This contract is compatible with OpenZeppelin Contracts ^5.0.0 and requires Solidity ^0.8.20.

### Usage

#### Installation

To use this contract, you need to import it into your project along with the required dependencies from OpenZeppelin Contracts.

#### Configuration

- Set the maximum supply of tokens by modifying the `maxSupply` variable.
- Configure the base URI for token metadata by modifying the `_baseURI` function.
- Adjust the minting requirements and costs in the `publicMint` and `allowedList` functions.

#### Functions

- `pause`: Pauses the contract. Only callable by the contract owner.
- `unpause`: Unpauses the contract. Only callable by the contract owner.
- `publicMint`: Allows public minting of tokens, subject to specified conditions.
- `allowedList`: Allows minting by specified addresses, subject to verification and conditions.
- `abletoMintByOwner`: Enables or disables minting permissions for specific lists. Only callable by the contract owner.
- `addToMinters`: Adds addresses to the list of authorized minters. Only callable by the contract owner.
- `isVerifiedToMint`: Checks if an address is authorized to mint tokens.
- `withdraw`: Withdraws the contract's balance to a specified address.

### License

This project is licensed under the MIT License.

### Disclaimer

This software is provided as-is, without any warranties or guarantees. Use it at your own risk.

### Credits

- OpenZeppelin Contracts: https://openzeppelin.com/contracts/