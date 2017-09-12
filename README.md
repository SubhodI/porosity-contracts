
## [Crowdsale](#1-crowdsale)

## [Lifecycle](#2-lifecycle-contract)

## [Math](#3-math-contract)

## [Ownership](#4-ownership-contract)

## [Payment](#5-payment-contract)

## [Token](#6-token-contract)

## [Bounty](#7-bounty-contract)

## [DayLimit](#8-daylimit-contract)

## [EC recovery](#9-ecrecover-contract)

## [Limit balance](#10-limit-balance-contract)

## [Multisig wallet](#11-multisigwallet-contract)

## [Reentrancy guard](#12-reentrancy-guard-contract)
## 1. Crowdsale
***
Crowdsale is a  contract for managing a token crowdsale.Crowdsales have a start and end block, where investors can make token purchases and the crowdsale will assign them tokens based on a token per ETH rate. Funds collected are forwarded to a wallet as they arrive.
    
### 2. Lifecycle contract
***
Lifecycle contract includes following solutions
* Fund management in case of contract destruction.
* Emergency stop mechanisms.

### 3. Math contract
***
Math contract includes following solution
* Checks for overflow/underflow of uint256 math operations.

### 4. Ownership contract
***
ownership contract includes following solution
* Controlling ownershipof the contract.
* Claming ownership of the contract.
* To block incoming ether to prevent accidental loss of Ether.
* This blocks incoming ERC23 tokens to prevent accidental loss of tokens.
* Interface contract for multisig proxy contracts.
* Solves a class of errors where a contract accidentally becomes owner of Ether, Tokens or Owned contract.
* Shareable contract : Number of approvals required(multiple owners) for particular action to be performed.

### 5. Payment contract
***
Payment contract includes following solution
* Supporting async send for pull payments.

### 6. Token contract
***
Token contracts has many different token safety checks. provides interface for ERC20 tokens. Refer each contract description for its use and security parameters.

### 7. Bounty contract
***
Bounty contract is a bug bounty contract where contract will pay out to a researcher who has successfully broken the target contract code/logic.

### 8. DayLimit contract
***
Base contract that enables methods to be protected by placing a linear limit (specifiable) on a particular resource per calendar day.

### 9. ECrecovery contract
***
Use recover function of this contract to get the Ethereum address of the signer.

### 10. Limit balance contract
***
Inherit this contract if you want to limit the balance of the contract.

### 11. MultisigWallet contract
***
Inherit this contract if you want to limit the balance of the contract.

### 12. Rentrancy guard contract
***
Use the modifier `nonReentrant` to make any function secure against re-entrancy attack.