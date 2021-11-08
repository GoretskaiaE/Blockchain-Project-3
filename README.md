# Ethereum Dapp for Tracking Items through Supply Chain

The supply chain smart contract allows to track the authenticity of coffee beans.

Starter code is here 
https://github.com/udacity/nd1309-Project-6b-Example-Template

Contract address on the Rinkeby Network: 0x0261A366a8F1CFcDE9cF33F01c195a8F24EC52CA

Transaction ID: 0x9da8a9e26d9b05c633672d0a2a6fafcf86c04048b8f49b0a435cdba489fd8f9f

Truffle version: Truffle v4.1.14

Solidity v0.4.24 (solc-js)

Node v10.16.3

## Libraries
Truffle allows to test smart contracts and migrate them to the Ethereum blockchain.

web3.js allows DApp to interact with contracts deployed to the Ethereum blockchain.

## UML diagrams
![Activity Diagram](/Diagrams/Activity.jpg)
![Sequence Diagram](/Diagrams/Sequence.jpg)
![State Diagram](/Diagrams/State.jpg)
![Data Model Diagram](/Diagrams/DataModel.jpg)

## How to test locally
Open Ganashe

```bash
truffle migrate
truffle test

cd app
npm run dev
```

Open http://localhost:3000/ in browser with installed Metamask 

Import an account, that is the owner of the contract, from Ganache to Metamask

Connect the account to http://localhost:3000/ in Metamask

Harvest, process, pack, sale, buy, ship, receive, purchase coffee!

Also, you can add farmers, distributors, retailers, consumers, import appropriate accounts from Ganache to Metamask, and test the DApp with different roles.

## Appendix
Output after truffle migrate --reset --network rinkeby
```bash
Using network 'rinkeby'.

Running migration: 1_initial_migration.js
  Deploying Migrations...
  ... 0x79e15cc1aec4fa4f5634b0ee341b0cf002bbc8c3fc53ac854c7569f5be9ac9e3
  Migrations: 0xff8d930d4021fad4371964ce480b3319c2ed7fb6
Saving successful migration to network...
  ... 0xeb63a7597458e8dedafb14b32c8138127c0fa8e7ff7fdf32f68133e668590548
Saving artifacts...
Running migration: 2_deploy_contracts.js
  Deploying FarmerRole...
  ... 0xf456b5323b989a9ffcd905036cf7575513b8f4e30ac661daef37b5c1e0dd41cd
  FarmerRole: 0xc88055d0f495ce9e7c184ca0ebea5c5f5b5090ca
  Deploying DistributorRole...
  ... 0x0ab702377da4e351d53931d338226731334ea8efcfaaae0359a44b85a6f6744a
  DistributorRole: 0x134ec25d52b946803cc13dcb26889fb590b84b55
  Deploying RetailerRole...
  ... 0xc374d281aae09c24384e9d37a02a33f4477553555a9c419697182a6783718add
  RetailerRole: 0x4eff43bd77a21b935517fdd27b3dd17f901a3d75
  Deploying ConsumerRole...
  ... 0x5df2a882d2c60b5a6d963631c42324145b579ce98d208091e3c4fc25f77a1d96
  ConsumerRole: 0xcdb06c7b09e1f8938d920572389fef320f134455
  Deploying SupplyChain...
  ... 0x9da8a9e26d9b05c633672d0a2a6fafcf86c04048b8f49b0a435cdba489fd8f9f
  SupplyChain: 0x0261a366a8f1cfcde9cf33f01c195a8f24ec52ca
Saving successful migration to network...
  ... 0x7963c68ef31d262aa89cc702f690de8dc46bb60e023bf428bf2d61c915a3eb6c
Saving artifacts...
```
