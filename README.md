# NFT-ERC721-using-hardhat

- To setup a Hardhat project, Open up the project directory in terminal and execute these commands

`npm init --yes`
`npm install --save-dev hardhat @nomicfoundation/hardhat-tool`

- In the same directory where you installed Hardhat run:

`npx hardhat`
Select `Create a Javascript Project` and follow the steps. At the end, you will have a new Hardhat project ready to go!

## Write NFT Contract Code

- Let's install some OpenZeppelin contracts so we can get access to the ERC-721 contracts. In your terminal, execute the following command:

`npm install @openzeppelin/contracts`

- Compile the contract, open up a terminal and execute these commands

`npx hardhat compile`

## Configuring Deployment

- `.env` file should look like :
`QUICKNODE_HTTP_URL="add-quicknode-http-provider-url-here"`
`PRIVATE_KEY="add-the-private-key-here"`
- Now we would install dotenv package to be able to import the env file and use it in our config. In your terminal, execute these commands.

`npm install dotenv`

- To deploy in your terminal type:

`npx hardhat run scripts/deploy.js --network goerli`
