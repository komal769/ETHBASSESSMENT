# MyToken Ethereum Token Project

## Overview

MyToken is an Ethereum smart contract that facilitates the creation and management of a custom ERC20 token. It provides functionalities for token creation, minting, burning, and balance management.

## Features

- **Token Details**: Includes public variables for token name (`name`), symbol (`symbol`), and total supply (`totalSupply`).
- **Balances Mapping**: Utilizes a mapping (`mapping(address => uint256) public balances`) to track token balances for each address.
- **Mint Function**: Increases the total token supply and adds tokens to a specified address.
- **Burn Function**: Decreases the total token supply by removing tokens from a specified address, with validation to ensure sufficient balance.

## Requirements

1. **Public Variables**: Store token details (`name`, `symbol`, `totalSupply`).
2. **Balances Mapping**: Track balances using `balances` mapping.
3. **Mint Function**: Increases `totalSupply` and updates `balances` for the recipient.
4. **Burn Function**: Decreases `totalSupply` and updates `balances` for the sender, with balance validation.

## Installation

To deploy and interact with MyToken contract using Remix IDE, follow these steps:

1. **Open Remix IDE**:
   - Navigate to [Remix IDE](https://remix.ethereum.org/).

2. **Create New File**:
   - Create a new Solidity file named `MyToken.sol`.

3. **Paste Contract Code**:
   - Copy and paste your `MyToken.sol` contract code into the Remix editor.

4. **Compile Contract**:
   - Click on the Solidity compiler icon on the left sidebar.
   - Select the appropriate compiler version (e.g., ^0.8.0).
   - Compile your contract by clicking on the "Compile" button.

5. **Deploy Contract**:
   - Switch to the "Deploy & Run Transactions" tab.
   - Select your contract (`MyToken`) from the dropdown.
   - Configure deployment parameters (token name, symbol, total supply).
   - Deploy the contract to a local development environment or a testnet like Ropsten.

## Usage

Once deployed, interact with the contract using Remix IDE:

1. **Interact with Contract**:
   - In the "Deployed Contracts" section, you'll see your deployed contract instance (`MyToken`).
   - Use the provided interface to interact with functions such as `mint` and `burn`.

2. **Example Transactions**:
   - Example of minting tokens:
     ```solidity
     // Mint 1000 tokens to address '0xAddress'
     MyToken.mint('0xAddress', 1000);
     ```

   - Example of burning tokens:
     ```solidity
     // Burn 500 tokens from address '0xAddress'
     MyToken.burn('0xAddress', 500);
     ```

## Smart Contracts

The contract `MyToken.sol` defines the token logic including minting and burning functionalities.

## Development

For further development and testing in Remix IDE:

- Ensure you have Solidity compiler (version ^0.8.0) selected.
- Utilize Remix's built-in tools for debugging, testing, and deploying contracts.

## Contributing

Contributions are welcome! Fork the repository and submit a pull request with your proposed changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For questions or support, please contact [Komal](jangrakomal06@gmail.com).
