# biteasy-unofficial

[![Version](http://img.shields.io/npm/v/biteasy-unofficial.svg)](https://www.npmjs.org/package/biteasy-unofficial)

A Biteasy adapter built to standardize the output of requests to follow the common-blockchain convention. Aliases are introduced in the return of functions to account for differences in convention between the two standards. It is our hope that the Bitcoin community will come to an agreement on proper style and convention for requests on addresses, transactions, and blocks. 

[Information on common-blockchain for convention](https://github.com/common-blockchain/common-blockchain/blob/master/README.md)

## Installation

Install as you normally install an npm module:
```
  npm install biteasy-unofficial
```

## Usage

Run ``` npm install ``` to have all necessary node modules installed.

To use the Biteasy API, simply require the module.
```javascript
  var biteasyAPI = require('biteasy-unofficial');
  var commonBlockchain = biteasyAPI({ network: 'mainnet' });
```
For Mainnet, use ```biteasyAPI({ network: 'mainnet' })``` when calling a function. For Testnet, use ```biteasyAPI({ network: 'testnet' })``` when calling a function. By default, if no parameter is provided, Mainnet will be used.

## API

[See abstract-common-blockchain for API](https://github.com/blockai/abstract-common-blockchain/blob/master/README.md)

## Examples

There are examples for using Addresses, Blocks, and Transactions, provided in the /examples folder. Each function includes a Mainnet and Testnet sample call and where possible, an invalid example is provided to show error handling. Expect all returns to be of the form (error, response).

## Convention

Standard convention is described fully by common-blockchain in the ```types.json``` file: https://github.com/blockai/common-blockchain/blob/master/types.json

## Maintainers
  * Howard Wu (howardwu) - howardwu@berkeley.edu
  * Andrew Malta (andrewmalta13) - andrew.malta@yale.edu
