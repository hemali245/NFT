# NFT minting and connecting it with Metamask

NFT stands for Non Fungible token and simply means that quality of asset that is similar but not exchangeable.

## ERC721 standard 


Alchemy for web3 \
Metamask used for interaction - Goerli Test Network \
Pinata used to upload image to IPFS 


Kindly follow below steps in order to create your snart contract and then connect with following : 

### Download Hardhat :
```bash
npm init
npm install --save-dev hardhat
npx hardhat
```
### Download preowned contracts from openzeppelin

```bash
npm install @openzeppelin/contracts
```

### Write your contract in Solidity which is MyNFT.sol

### Creation of .env file :
```python
# Mention below details in .env file from your Alchemy and Metamask account

API_URL=" "
PRIVATE_KEY=" "
```

### Install hardhat-ethers
```
npm install --save-dev @nomiclabs/hardhat-ethers 'ethers@5.0.0'
```

### Set up your deploy.js file and upload image to Pinata

```
npx hardhat run scripts/deploy.js --network goerli

# Now you should get your contract address
```

## Now your smart contract for NFT is deployed.

### Installing Alchemy-web3
```
npm install @alch/alchemy-web3
```

In mint-nft.js mention the following details :
```
Public Key -> Metamask Account Key
Private Key -> Metamask Test Network Private Key
Contract Address -> The contract address which is created.

# Transaction is created from public key to contract address
```
## Final Step to mint NFT
```
node scripts/mint-nft.js
```
### You can check minted NFT in Mobile Application of Metamask with following details:
Transaction ID as 1 \
Address as contract Address

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
