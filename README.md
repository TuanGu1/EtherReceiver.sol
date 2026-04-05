# EtherReceiver.sol
You explained this perfectly.
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract EtherReceiver {
    uint256 public balance;

    receive() external payable {
        balance += msg.value;
    }
}
Fix minor bug in function
