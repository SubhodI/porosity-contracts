
## [Crowdsale](#1-crowdsale)

## [Lifecycle](#2-lifecycle-contract)

## [Math](#3-math-contract)

## [Ownership](#4-loan)

## [Payment](#5-access-control-using-modifiers)

## [Token](#6-contract-as-state-machine)

## [Bounty](#7-withdrawal-pattern-re-entrancy)

## [DayLimit](#8-prepare-for-failure)

## [EC recovery](#9-digital-locker-contract)

## [Limit balance](#10-solidity-libraries)

## [Multisig wallet](#10-solidity-libraries)

## [Reentrancy guard](#10-solidity-libraries)
## 1. Crowdsale
***
        Crowdsale is a  contract for managing a token crowdsale.Crowdsales have a start and end block, where investors can make token purchases and the crowdsale will assign them tokens based on a token per ETH rate. Funds collected are forwarded to a wallet as they arrive.
    
### 2. Lifecycle contract
***
        Lifecycle contract includes following solutions.
        * Fund management in case of contract destruction.
        * Emergency stop mechanisms.

### 3. Math contract
***
    Math contract

