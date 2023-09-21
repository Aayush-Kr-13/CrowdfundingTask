# CrowdfundingTask
CrowdFunding Smart Contract
Introduction
The CrowdFunding smart contract is designed to facilitate crowdfunding campaigns on the Ethereum blockchain. It allows users to contribute Ether to a campaign and manage fund distribution through a voting mechanism for proposed requests.

Features
Campaign Manager: The contract has a manager address who has the authority to create spending requests and finalize them.

Contribution Tracking: The contract tracks contributors and their contributions, ensuring that only contributors can participate in the voting process.

Spending Requests: Campaign managers can create spending requests that describe how funds will be used. These requests must be approved by a majority vote among contributors.

Refund Mechanism: Contributors can request refunds if the campaign did not meet its funding target before the deadline.

Getting Started
To deploy and interact with this contract, you can follow these steps:

Compile the Contract: Use a Solidity compiler compatible with the specified version (>=0.5.0 <0.9.0) to compile the CrowdFunding.sol smart contract.

Deploy the Contract: Deploy the compiled contract on the Ethereum network of your choice, specifying the target and deadline as constructor parameters.

Contribute Ether: Contributors can send Ether to the contract using the sendEth function. Contributions must meet the minimum contribution requirement.

Campaign Management:

The contract manager can create spending requests using the createRequests function.
Contributors can vote on spending requests with the voteRequest function.
The manager can finalize a spending request with the makePayment function if it has enough votes.
Refunds: If the campaign does not reach its funding target by the specified deadline, contributors can request refunds using the refund function.

Contract Balance: Use the getContractBalance function to check the current balance of the contract.

Important Notes
Ensure that you have a proper development and testing environment set up, such as Truffle or Remix.

Be cautious when deploying the contract to a live Ethereum network, as it involves real Ether transactions.

Remember to manage the manager address securely, as it has significant control over the contract.

Make sure to thoroughly test the contract on a testnet before deploying it on the main Ethereum network.

License
This code is provided under an "UNLICENSED" SPDX-License-Identifier. You can use and modify the code freely, but please note that there are no specific license terms provided.

You can enhance this README by including deployment instructions, a usage example, and any additional details you think are relevant to users and developers who want to interact with your smart contract.
