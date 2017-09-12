### 1. Crowdsale
***
Crowdsale is a contract for managing token crowdsale. Crowdsales have a start and end block, where investors can make token purchases and the crowdsale will assign them tokens based on a token per ETH rate. Funds collected are forwarded to a wallet as they arrive.
    
### 2. Lifecycle contract
***
Lifecycle contract has following mechanisms
* Fund management in case of contract destruction.
* Emergency stop mechanisms.

### 3. Math contract
***
Math contract Checks for `overflow/underflow` of uint256 basic math operations.

### 4. Ownership contract
***
ownership contract has following mechanisms
* Controlling ownershipof the contract.
* Claming ownership of the contract.
* To block incoming ether to prevent accidental loss of Ether.
* This blocks incoming ERC23 tokens to prevent accidental loss of tokens.
* Interface contract for multisig proxy contracts.
* Solves a class of errors where a contract accidentally becomes owner of Ether, Tokens or Owned contract.
* Shareable contract : Number of approvals required(multiple owners) for particular action to be performed.

### 5. Payment contract
***
Payment contract Supports async send for pull payments.

### 6. Token contract
***
Token contracts has many different token safety checks. provides interface for ERC20 tokens. Refer each contract description and code for its use and security parameters.

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
Contract can hold multiple owners address and number of approvals required for any trasnaction and it also has daily limit. Executes transaction immediately if below daily spending limit. If not, goes into multisig process.

### 12. Re-entrancy guard contract
***
Use the modifier `nonReentrant` to make any function secure against re-entrancy attack.