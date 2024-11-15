# Lisk L2
Lisk makes its transition to Layer 2, it’s essential to stay informed and prepared.
# Overview of Lisk L2
Lisk is transitioning from an L1 blockchain to an L2 solution built on Ethereum using the OP Stack technology. This migration aims to leverage Ethereum's security while providing improved scalability and lower fees for developers building applications. 

# Key Features and Benefits
Near-zero transaction fees (<$0.01), potentially 10-100x cheaper than Ethereum mainnet 
Superchain interoperability, allowing seamless asset transfers across major blockchain
 networks
 Built-in security from Ethereum's decentralized and secure settlement layer 
Full EVM equivalence, enabling developers to deploy existing L1 contracts on L2 without changes.

![image](https://github.com/user-attachments/assets/2dfd7e9c-e9af-4dd0-8e57-50bf56b19e41)


## Installation
# Lisk L1-L2 migration guide

# Requirements
* A Lisk L1 application built on Lisk SDK version 6.0.0 or later
* Basic understanding of Solidity
* Smart contract development framework (Foundry used as example)
# Project Setup
Create a new project using Foundry:
```bash
  
forge init hello_liskl2
cd hello_liskl2
  
```
Create a new smart contract file (e.g., Hello.sol):
```bash
pragma solidity ^0.8.20;

contract Hello {
  // State variables
  mapping(address => string) public message;
  uint32 public counter = 0;
  
  // Events
  event NewHello(address indexed sender, string message);
  
  // Functions
  function createHello(string calldata _message) public {
    message[msg.sender] = _message;
    counter += 1;
    emit NewHello(msg.sender, _message);
  }
}
  
```
# Migration Steps
1 Migrate module-specific configurations to state variables in the smart contract

2 Implement custom modifiers for verification (e.g., validLength, validWords)

3 Create view functions for endpoints

4 Test the smart contract locally

5 Deploy the smart contract to Lisk L2

# Testing and Deployment
* Write tests for the smart contract (e.g., Hello.t.sol)
* Run tests with forge test
* Deploy the smart contract using forge create with the appropriate flags

# Post-Migration Steps
* Interact with the deployed smart contract
* Migrate plugins and UI of the Lisk L1 app to be compatible with the new API

# Additional Resources
* Official Lisk Portal: https://portal.lisk.com/

* Lisk Bridge: Official bridge for transferring assets between chains

* Relay Bridge: Alternative third-party bridge service

Remember to always verify information from official sources and never assume details. The migration process requires careful planning and execution to ensure a smooth transition from Lisk L1 to Lisk L2
# A Sneak Peek at the Lisk Airdrop: How It Works and What’s Coming
Following the successful launch of our User Mainnet, we’ve designed our Airdrop with multiple ways to participate. From flexible tasks you can complete at your own pace to unique partner challenges and even dapp-exclusive opportunities, here’s a preview on how to get involved and what to expect once the campaign goes live on November 21st: 
# Earn Points by Completing Tasks
All participants can earn points by completing a range of activities on the Lisk Portal. The more tasks you complete, the more points you accumulate, which will determine the total LSK tokens you receive at the end of the campaign period.

Task Categories:

Platform Tasks: Get hands-on with Lisk’s features through simple platform activities.
Educational Tasks: Learn more about Lisk and web3 tech with these quick, informative tasks.
Engagement Tasks: Connect with the community in discussions and events, sharing your ideas and meeting others.
#  Check Out Partnership-Driven “Super Tasks” for Immediate Rewards
To make things even more exciting, we’ve teamed up with partners like Oku.Trade, Ionic, Creo Engine, Angle Protocol, Soccersm, and Momint. Each partner will host a two-week period with unique “Super Tasks” that provide immediate rewards. Unlike the points-based tasks, Super Tasks allow you to unlock LSK tokens on the spot, adding a layer of instant gratification to your journey in the Lisk ecosystem. These limited-time tasks are designed to add excitement and keep things dynamic as you progress.
# Follow our social media
https://x.com/LiskHQ

https://www.linkedin.com/company/lisk/
