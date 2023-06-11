## Introduction

Solidity is a high-level programming language used for implementing smart contracts on various blockchain platforms like Celo. This challenge focuses on developing a secure wallet contract using Solidity.

## Problem Statement

Create a secure wallet contract with the following requirements:

1. The wallet contract should allow deposits.
2. The contract should allow withdrawals only to the wallet owner.
3. The contract should provide a mechanism to change the wallet owner.
4. Implement a way to check the current balance of the wallet.
5. Implement a way to log all transactions, both deposits, and withdrawals.

## Hints

- Use state variables to store the wallet balance, the owner's address, and transaction logs.
- Utilize the `msg.sender` global variable to handle deposits, and owner-based function calls.
- Use `require()` to enforce contract rules, such as ensuring only the owner can withdraw or change the owner's address.
- Implement an event to log all transactions for transparency and traceability.
- Keep track of each transaction with a `struct` and save them in an array or mapping for logging purposes.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and satisfy all requirements.
- **Readability**: The contract should be well-structured with clear, commented code for easy understanding.
- **Testability**: Include examples of how to test each function of the contract.

Bear in mind that this challenge does not cover several crucial aspects such as gas optimization, contract upgradability, or security measures against reentrancy attacks. These are vital considerations for a real-world wallet contract.

To deepen your understanding of Ethereum smart contracts and Solidity, consider reading through the Celo and Solidity tutorials.

## Submission

Please provide a link to your PR on GitHub, including your secure wallet contract. Also include any notes, comments, or design choices you think are important for understanding your contract. Lastly, provide a brief explanation of how to test each function in the contract.
