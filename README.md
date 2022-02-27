# Basic ProxyFactory

## Storage.sol
Basic storage contract that can store ```string```, ```uint``` & ```bool``` and then retrieve the saved variables.

## StorageFactory.sol
Using OpenZeppelin [ProxyFactory.sol](https://github.com/OpenZeppelin/openzeppelin-sdk/blob/master/packages/lib/contracts/upgradeability/ProxyFactory.sol) creates new implementations of **Storage.sol** contract.


## How To Use
1. Deploy instance of **Storage.sol**.
2. Deploy instance of **StorageFactory.sol** which requires the address of **Storage.sol**.
3. Call ```clone()``` to get a new implementation of **Storage.sol** (address of new implementation emitted in clone event).