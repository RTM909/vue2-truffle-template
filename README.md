# Vue2 & Truffle Template
 
## Description 
This is a template application for Truffle with Vue2. This template contains VueX, Vue-Router and support for SCSS syntax in-built.

## Functions Included 
- Web3 Library & MetaMask  
- Multiple Account support through MetaMask included 
 

## Dependencies 
- [Node Js](https://nodejs.org/en/download/) - Network Architecture
- [Truffle](https://www.trufflesuite.com/truffle) - Framework
- [Ganache](https://www.trufflesuite.com/ganache) - Creation of Private Blockchain 
- [OpenZeppelin Library](https://github.com/OpenZeppelin/openzeppelin-contracts) - ERC721 Contract 
- [VueJS](https://vuejs.org/) - Front-End
- [Solidity Ver 8+](https://docs.soliditylang.org/en/v0.8.4/) - Back-End 
- [MetaMask](https://metamask.io/download) - Wallet & web3 provider 

## Setup (windows demo environment) 
 
- Download the project 
- Next, do this in both the `root` folder as well as the `vapp` folder  for installing all dependencies

  ```
  npm install
  ```
- After the dependencies are successfully installed open `Ganache`
- Quickstart a new Ethereum environment 
- Now check the RPC server for the port number, it should look something like `http://127.0.0.1:3454` in which `3454` is the port number
- Verify it in the `truffle-config.js` file in the project 
- Execute the command in the terminal 

  ```
  truffle migrate
  ```
- After successful compilation and contract migration, execute this command in the `vapp` folder
  
  ```
  npm run serve
  ```
- This will run the Dapp development server on ` http://localhost:8080/` 

### Connecting MetaMask to Dapp 
1. Install the [MetaMask](https://metamask.io/download) browser extension
2. Setup a new wallet account
3. Go to Ganache and copy the `RPC Server` Address in the top panel

   > You need this to import your Ganache Blockchain into MetaMask
4. Go to MetaMask and click on the networks tab (This should be selected as Ethereum Mainnet or some testnet such as Rinkeby)
5. Select `Custom RPC` in this tab at the bottom
6. Enter the name of your choice, the `RPC Address` that you copied, and `1337` as the chain ID
7. Other details should be auto-filled after entering the above details
8. Click on save and you should have the Ganache network in your MetaMask now
9. Then go to Ganache and click on the 🔑  on the right of the account number
10. Copy the `Private Key` which would look something like this 
  ```
  357e626beea4019ee4ca96c1234ed52e390b71c6db0c64d15cdee1cc68a57aef
  ```
11. Now open MetaMask and click on your account image and click `Import account`
12. Paste the copied private key in this and press on `Import`
 > Note: The `Quickstart Ethereum` you started in Ganache is temporary and every account that was generated will be lost forever once you close Ganache. You will have to do the steps `9 to 12` every time you open ganache. You will have to save the Workspace in Ganache if you wish to prevent this.
- Now reload the page
- MetaMask should popup asking you to connect your account
- If you connected successfully, your wallet address should be visible in the app. E.g.: `0xC9b87aeC184293A1D6d79806c8a0D70921090921`

### License
**MIT**

