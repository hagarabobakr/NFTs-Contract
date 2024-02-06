# DAWAM - Decentralized Artwork Minting

This repository contains a Solidity smart contract for creating Non-Fungible Tokens (NFTs) using OpenZeppelin and Alchemy.

## Overview

**DAWAM** (Decentralized Artwork Minting) is a Solidity smart contract that enables the creation and management of NFTs on the Ethereum blockchain. This contract utilizes the OpenZeppelin library for ERC721 token standards and Alchemy for Ethereum node interactions.
## Screenshots
<div>
  <img src = "https://github.com/hagarabobakr/NFTs-Contract/assets/84254977/690f4231-e997-41a8-a89e-779e7fa1ac4f" width = "800">
  <img src = "https://github.com/hagarabobakr/NFTs-Contract/assets/84254977/9e828b48-3277-4df0-8e22-379b85780597" width = "800">
</div>
<div>
  <img src = "https://github.com/hagarabobakr/NFTs-Contract/assets/84254977/313b06f3-3fc3-44b0-8d79-e71bb51e7877" width = "800">
  <img src = "https://github.com/hagarabobakr/NFTs-Contract/assets/84254977/02867f72-0011-4eb3-9bd5-f36238b8127e" width = "800">
</div>

## Features

- ERC721 Compliance: Implements the ERC721 standard for non-fungible tokens.
- Minting Functionality: Allows the owner to safely mint new tokens with unique metadata URIs.
- Token URI Management: Supports storing and retrieving metadata URIs for each token.
- Ownership Control: Utilizes Ownable contract to manage ownership of the NFT contract.

## Prerequisites

Before deploying or interacting with this smart contract, ensure you have the following:

- Ethereum Wallet (e.g., MetaMask) configured with an Ethereum account.
- Access to an Ethereum node (e.g., via Alchemy API).
- Basic understanding of Ethereum smart contracts and NFTs.

## Deployment

To deploy this contract, follow these steps:

1. Compile the contract using a Solidity compiler (e.g., Remix IDE, Truffle).
2. Deploy the compiled contract to the Ethereum network using a deployment tool or script.
3. Interact with the deployed contract using its address and ABI (Application Binary Interface).

## Usage

### Minting Tokens

To mint new tokens, the contract owner can call the `safeMint` function with the desired recipient address and metadata URI.

```solidity
function safeMint(address to, string memory uri) public onlyOwner {
    // Implementation details
}
```

### Metadata URI

The contract stores metadata URIs for each token. The `tokenURI` function allows retrieving the metadata URI for a specific token ID.

```solidity
function tokenURI(uint256 tokenId) public view returns (string memory) {
    // Implementation details
}
```

## Dependencies

- **OpenZeppelin Contracts**: Provides implementation for ERC721 token standards and other utilities.
- **Alchemy**: Ethereum node provider for interacting with the Ethereum blockchain.


## Acknowledgments

- OpenZeppelin Team
- Alchemy Team

## Support

For any inquiries or issues regarding this contract, please open an issue on the GitHub repository.
