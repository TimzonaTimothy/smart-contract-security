# SMART CONTRACT SECURITY

This repository houses the streamlined and minimalist audit report for the Metacrafters security task. It includes the rectified and updated code, previously vulnerable, now rewritten in a more recent version of Solidity, with all identified bugs successfully addressed.

## Description


This codebase features a basic contract written in Solidity, the programming language for Ethereum smart contracts. The "StorageVictim" contract has 1 critical vulnerability, 1 medium vulnerability, and 2 informational vulnerabilities.

## Findings/Suggestions 

    Change the compiler version
    Change the function StorageVictim() public to contructor() public
    update address owner to address public owner
    In the store function, directly update storages[msg.sender] without creating a local struct.

### Getting Started

## Clone the repository:

   git clone <repository_url>
  

## Install Dependencies:

    npm install

## Compile the contract:

    npx hardhat compile

## Deploy the contract:

    npx hardhat run scripts/deploy.js --network mumbai

## Verify the contract:

    npx hardhat run scripts/verify.js --network mumbai


Running the contract with hardhat:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat compile
npx hardhat run scripts/deploy.js --network mumbai
npx hardhat run scripts/verify.js --network mumbai
```