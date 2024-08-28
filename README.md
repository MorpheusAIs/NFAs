# NFAs
## Non Fungible Agents 
## Status: In Development / Testing

### The NFA Standard was first described in MRC 21. Credit to MaxwellSmartAgent.
https://github.com/MorpheusAIs/MRC/blob/main/IN%20PROGRESS/MRC21.md

### Technical Documentation Available on Notion: 
https://nounspace.notion.site/MRC21-Factory-Guide-c5c0c48039a2499eaebf5b54c731ed20

## MRC21 Factory Guide
The NFA Factory contract enables developers to deploy an NFA contract. An NFA Contract is an ERC721 with the following metadata on the developers agent/application:

### **BasicInfo**

- **Name:** `Example Name`
- **Symbol:** `EXN`

### AppInfo

- **Router Required:** `Checked`
- **Payment Model:** `subscription`
- **Download URIs:** `https://example.com/download1,https://example.com/download2`
- **Code Hash:** `0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef`
- **ABI URIs:** `https://example.com/abi1,https://example.com/abi2`
- **ABI Hash:** `0xabcdef1234567890abcdef1234567890abcdef1234567890abcdef1234567890`
- **Version ID:** `1.0`

### VersionInfo

- **Version ID:** `1.0`
- **Download URIs:** `https://example.com/download1,https://example.com/download2`
- **Code Hash:** `0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef`
- **ABI URIs:** `https://example.com/abi1,https://example.com/abi2`
- **ABI Hash:** `0xabcdef1234567890abcdef1234567890abcdef1234567890abcdef1234567890`

### Initial Owner

- **Initial Owner Address:** `0xYourInitialOwnerAddress` (Replace with a valid Ethereum address, e.g., `0x1A2b3C4d5E6F7890aBCdEf1234567890AbcDEf12`)

## Here is the NFA Factory contract on Sepolia Testnet:
https://sepolia.etherscan.io/address/0xe2e43ef883ff83307627c92153c9c356821aff9b

Here is a UI where you can connect Metamask (or any injected wallet) and create an NFA contract on Sepolia Tesnet: https://codepen.io/willyo11/pen/gOJRzBg

Final adjustments we’re proposing for the v0 contract (which is also upgradeable currently)
1. Add optional description field to BasicInfo

1. Add optional tags field to BasicInfo (enables tag standards to be developed and interfaces to decide if/how to consume)
2. Add optional image
3. Add the ability to set a mint price (in eth) when deploying an NFA from the factory. If a mint price is set, users must pay the mint price in order to mint the NFA.
    1. The reason for this is that it would provide developers with a built in monetization strategy (albeit only for one-time or initial payments) as well applications with the ability to token-gate access to to NFAs (if they want).

## Example Front End
- https://codepen.io/willyo11/pen/gOJRzBg
