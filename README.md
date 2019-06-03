# Real Estate Project - Udacity Blockchain Capstone
This is a ERC721 sample application for Udacity's Blockchain course. 

## Getting Started

## Installing


#### Install required node packages 
Change to project folder and install all requisite npm packages (as listed in ```package.json```):

```
npm install
```

#### Open a  terminal window and Launch Ganache:
If you are using ganache-cli use this command to add 40 funded accounts:

```
ganache-cli -p 8545 -m "spirit supply whale amount human item harsh scare congress discover talent hamster" --gasLimit 300000000 --gasPrice 20000000000 -a 40

```

#### Open a separate terminal window and  compile smart contracts:
cd /eth-contracts

```
truffle compile
```

#### ABI's link:

This will create the smart contract artifacts (ABI files) in folder ```/eth-contracts/build/contracts```.

#### Migrate smart contracts to the locally running blockchain, ganache:
Change to the folder ```eth-contracts```

```
truffle migrate
```
This will :
  - deploy the smart contract artifacts to running Ganache 
 
#### Test smart contracts:
Change to the folder ```eth-contracts``` 
```
truffle test ./test/TestERC721Mintable.js 
```

![TestERC721Mintable.js](/images/TestERC721Mintable.png)

```
truffle test ./test/TestSolnSquareVerifier.js  
```

![TestSolnSquareVerifier.js](/images/TestSolnSquareVerifier.png)


```
truffle test ./test/TestSquareVerifier.js  
```

![TestSquareVerifier.js](/images/TestSquareVerifier.png)


#### Deploying contracts to rinkeby
##### Following contracts are deployed to rinkeby for this project:
* Deploying 'Verifier'

    contract address(click to view on etherscan):
    [0x8895c95A99a9C34e86C3473443Bd7d903c8aDd25](https://rinkeby.etherscan.io/address/0x8895c95A99a9C34e86C3473443Bd7d903c8aDd25)

* Deploying 'SolnSquareVerifier'

    contract address(click to view on etherscan):
[0xCC539Dc3fC1eb46844844dc4B0Df7bA609F78c81](https://rinkeby.etherscan.io/address/0xCC539Dc3fC1eb46844844dc4B0Df7bA609F78c81)


#### Mint tokens
[Real Estate Token](https://rinkeby.etherscan.io/token/0xCC539Dc3fC1eb46844844dc4B0Df7bA609F78c81)
##### For this project :
![](/images/minttoken.png)
#### Generate Storefront on OpenSea marketplace:
OpenSea has a Rinkeby environment that allows developers to test their integration with OpenSea. 
![OpenSea submit marketplace page](/images/opensea_front.png)

#### Test and Verify OpenSea with  SolnSquareVerifier tokens:

https://rinkeby.opensea.io/category/realestatetokenv6


## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.
* [ZoKrates](https://github.com/Zokrates/ZoKrates) - Implement zkSnarks using ZoKrates, a toolbox for zkSNARKs on Ethereum.
* [Docker](https://docs.docker.com/install/) - Docker is the recommended way to get started with Zokrates. Docker is a tool designed to make it easier to create, deploy, and run applications by using containers.
* [OpenSea](https://docs.opensea.io/docs) - OpenSea is a decentralized marketplace that is used for selling for crypto assets
* [Infura](https://infura.io/) - Scalable Blockchain Infrastructure
* [Metamask](https://metamask.io/) - MetaMask is a bridge that allows to visit the distributed web in browser.