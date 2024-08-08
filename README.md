# Joint Savings Account Smart Contract

![alt=“”](Images/20-5-challenge-image.png)

## Project Overview

A fintech startup is disrupting the finance industry with its own cross-border, Ethereum-compatible blockchain connecting financial institutions. The team is building smart contracts to automate various financial processes, including joint savings accounts.

This repository contains the project files for the Joint Savings Account smart contract developed as part of a fintech startup's initiative to disrupt the finance industry. This project focuses on integrating Ethereum blockchain technology to automate the creation and management of joint savings accounts for financial institutions.

### Objectives

- **Create a Joint Savings Account Contract in Solidity:** Develop a Solidity smart contract that accepts two user addresses, allowing them to control a joint savings account.
- **Ether Management Functions:** Implement functions to deposit and withdraw funds, ensuring secure and efficient ether management.

## Technology and Tools

- **Solidity:** Programming language used to write the smart contract.
- **Remix IDE:** Integrated development environment for writing, compiling, and deploying Solidity smart contracts.
- **JavaScript VM:** Virtual machine in Remix IDE used for deploying and testing the smart contract.
- **Ethereum:** Blockchain platform that supports the execution of the smart contract.

## Smart Contract Details

### JointSavings Contract

The `JointSavings` smart contract includes the following features:

- **Variables:**
  - `address payable accountOne` and `address payable accountTwo`: The two user addresses authorized to control the joint savings account.
  - `address public lastToWithdraw`: The last address that made a withdrawal.
  - `uint public lastWithdrawAmount`: The amount of the last withdrawal.
  - `uint public contractBalance`: The current balance of the contract.

- **Functions:**
  - `withdraw(uint amount, address payable recipient)`: Allows the authorized addresses to withdraw funds, with checks for account ownership and sufficient balance.
  - `deposit() public payable`: Allows ether to be deposited into the contract.
  - `setAccounts(address payable account1, address payable account2)`: Sets the two authorized user addresses.
  - Fallback function to store ether sent from outside the `deposit` function.

## Execution Results

The project includes a folder named `Execution_Results` containing images that confirm the successful execution of deposit and withdrawal transactions in the JavaScript VM. These images demonstrate the functionality and reliability of the `JointSavings` contract.

## Instructions

### Step 1: Create a Joint Savings Account Contract in Solidity

1. Define the `JointSavings` contract with the necessary variables and functions.
2. Implement the `withdraw` function with require statements and ether transfer logic.
3. Implement the `deposit` function to update the contract balance.
4. Add a function to set the user addresses.
5. Include a fallback function for external ether transfers.

### Step 2: Compile and Deploy Your Contract in the JavaScript VM

1. Compile the smart contract in the Remix IDE.
2. Deploy the contract using the JavaScript VM environment in Remix.

### Step 3: Interact with Your Deployed Smart Contract

1. Use the `setAccounts` function to define the authorized addresses.
2. Test the `deposit` functionality by sending various amounts of ether.
3. Test the `withdraw` functionality by withdrawing specified amounts to the authorized addresses.
4. Verify the contract balance and withdrawal details after each transaction.

## Conclusion

This project demonstrates the implementation of a secure and efficient joint savings account smart contract using Solidity. By leveraging Ethereum's blockchain technology, the fintech startup enhances the automation and reliability of financial processes for its users.

---


