# Remix Ethereum IDE

This Solidity program is a simple starting point for those who are new to Solidity and want to get a feel for how it works.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. So this is just a simulation of free-making of our very own token. For the first part, I need my contract as "My Token". Next, I declare make-up variables in which stores the details about my token. Which are streaming for token name abbreviation. string every important domain of the creation and supply used the int so that and then I just put the values of this one. I did variables, which is JOHN and JHN for abbreviation and lastly i set the supply to 0. After that I used the mapping function to get the token of the address,
## Getting Started

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

I input my code there 

``` // SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

contract MyToken {

    // public variables here
string public tokenName = "John";
string public tokenAbbrv = "JHN";
uint public totalSupply = 0;
    // mapping variable here
 mapping(address =>uint) public balances;
    // mint function
function mint (address _address, uint _value) public {
    totalSupply += _value;
    balances [_address] += _value;
}
    // burn function
function burn (address _address, uint _value) public {
    if (balances[_address] >= _value) {
    totalSupply -= _value;
    balances [_address] -= _value;
    }
}
}
```


