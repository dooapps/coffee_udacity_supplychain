# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)

# UML

![truffle test](images/sequence.png)

![truffle test](images/state.png)

![truffle test](images/activity.png)



## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

> The starter code is written for **Solidity v0.4.24**. At the time of writing, the current Truffle v5 comes with Solidity v0.5 that requires function *mutability* and *visibility* to be specified (please refer to Solidity [documentation](https://docs.soliditylang.org/en/v0.5.0/050-breaking-changes.html) for more details). To use this starter code, please run `npm i -g truffle@4.1.14` to install Truffle v4 with Solidity v0.4.24. 

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/udacity/nd1309/tree/master/course-5/project-6
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "during report attitude sort group discover under neck affair local airport tired"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)


Running migration: 1_initial_migration.js
  Replacing Migrations...
  ... 0xa6a290c9c381c2827398bdffd2a2b33c19b4cabc363df9398c68896044deaeb0
  Migrations: 0xfcc61672aefd43d26c06eece753df5bdeebc4231
Saving successful migration to network...
  ... 0x414fcd544644d6feede698d8ab5ead98c2f1d6daaa03f4bd4f24cbca59055a9c
Saving artifacts...
Running migration: 2_deploy_contracts.js
  Replacing FarmerRole...
  ... 0x14f8994a366457d6f3caa0120742f95672acae95028de408ace6377b2065f3a4
  FarmerRole: 0xb7c03e3cbb506acbd5507a2422d82cbcf0d3abd4
  Replacing DistributorRole...
  ... 0x4a53a97c3cda58fa385815176bbff9871ef36987b4ccc41faefd97ec5327ffe2
  DistributorRole: 0xf4e9b7be10e2400f44e61cde872f4594c696a499
  Replacing RetailerRole...
  ... 0x5fd5e3231ad1ae65c7f32d9f6408bbc1549dbe632957f07bc4db5b0ea2787a2a
  RetailerRole: 0xd6df45f9164454cb88200ae0d2df98a8bd2b14f2
  Replacing ConsumerRole...
  ... 0xff0b6d5b82b725d528524bd9091812eb15051d246f4f1d3638ea0b7eb7947ed3
  ConsumerRole: 0x59fed39a8e400fcd0cc90a53818db734e9b28ba7
  Replacing SupplyChain...
  ... 0x530d4ef8b319c3591b289f91d99963482a2645e8dfd374d968fb17026437039c
  SupplyChain: 0xbc7af03aa3a689cfeeee62090e097a63779192b9
Saving successful migration to network...
  ... 0x434409c1ccdfc90eec5ae3cc6d19698d305211c8472980fbd072c7afd213d63e
Saving artifacts...


Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS
