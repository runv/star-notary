# Star Notary
### Simple DApp project
Demonstartes how to create ethereum DApp with it's own non-fungible token and basic front end functionality.

##### Table of Contents  
  * [Token](#token)
    + [Token Address](#token-address)
  * [Libraries](#libraries)
  * [How to install and run](#how-to-install-and-run)
    + [Deploy token to the local network](#deploy-token-to-the-local-network)
    + [Run Front End Application](#run-front-end-application)
      - [Open app in your browser](#open-app-in-your-browser)
        * [Interact with Token deployed locally](#interact-with-token-deployed-locally)
        * [Interact with Token deployed to rinkeby](#interact-with-token-deployed-to-rinkeby)
 

## Token

The Token implements ERC-721 specification and has its own Name and Symbol:

- ERC-721 Token Name = **MyStarToken**
- ERC-721 Token Symbol = **MYST**

### Token Address

**Token Address: 0x48A9a27EC2428BB28D4DE5d522439666A9017435** on the Rinkeby Network

## Libraries

The following libraries were used in order to implement this project:

- Truffle - v5.2.2 (core: 5.2.2)
- OpenZeppelin - v3.4.1
- Solidity - 0.7.4 (solc-js)

## How to install and run 

If you don't want to run your local version of network you can skip next part

### Deploy token to the local network
Install Truffle from https://www.trufflesuite.com/truffle
Go to root directory and run
```
npm install
truffle develop
compile 
migrate --reset
```
To run tests run additionally:
```
test
```
or
```
truffle test
```

### Run Front End Application
Go into the /app directory and run:
```
npm run dev
```
After that the local webpack server is started on your machine: http://localhost:8080/

#### Open app in your browser 
You need MetaMask version to be installed in your browser. You can download it from https://metamask.io/

##### Interact with Token deployed locally
In MetaMask choose Networks -> Custom RPC, then enter New RPC URL http://127.0.0.1:9545/. Import any account from truffle develop console. 
Open http://localhost:8080/ in your browser.

##### Interact with Token deployed to rinkeby

In MetaMask switch to rinkeby network and add an account if you don't have one. You also need some ether in that account. 
If you don't have go to the rinkeby ether faucet and request some ether.
After that add **MYST** Token into your MetaMask wallet.
Open http://localhost:8080/ in your browser.

