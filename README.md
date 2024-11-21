# Smart Contract Deployment Process

This document outlines the steps I followed to create, compile, and deploy smart contracts using Remix IDE and the Arbitrum Sepolia Testnet.

## 1. Setting Up the Workspace
- Opened Remix IDE and navigated to the file explorer.  
- Opened an existing folder named **Arbitrum Deployment** to use as a workspace.  
- Created three Solidity files:  
  - `StorageFactory.sol`  
  - `AdvancedStorage.sol`  
  - `ConflictExample.sol`

## 2. Writing the Smart Contracts
- Added a license identifier and specified the compiler directive version in each file.  
- Defined the contracts:
  - **`StorageFactory.sol` and `AdvancedStorage.sol`:**  
    - Declared a `uint256` variable named `favoriteNumber`.  
    - Used the `import` function to deploy instances of other contracts and pull their code.  
    - Made functions and variables public to allow external access.  
  - **`ConflictExample.sol`:**  
    - Created three functions: `parent1`, `parent2`, and `child`.  
    - Used inheritance and function overriding in the `child` function to resolve conflicts.

## 3. Compiling the Contracts
- Selected the Solidity compiler from the sidebar.  
- Ensured the compiler version matched the version specified in the contracts.  
- Clicked "Compile" and verified the success with a green checkmark.

## 4. Deploying and Testing the Contracts
- Navigated to the "Deploy & Run Transactions" tab.  
- Selected **Injected Web3 (MetaMask)** as the environment.  
- Deployed the `StorageFactory` contract.  
- Tested the contract by:  
  - Entering values into contract functions and observing responses.  
  - Testing data retrieval and updates on the **Arbitrum Sepolia Testnet**.

## Tools Used
- **Remix IDE**: For writing, compiling, and deploying smart contracts.  
- **MetaMask**: For Web3 integration and deploying on the Arbitrum Sepolia Testnet.  

This process ensures efficient development and testing of Solidity smart contracts.  
