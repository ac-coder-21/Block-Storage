Readme.txt

This is a detail steps for the execution of 'Block Storage' project by 
BEA126 Akash More
BEA128 Amogh Chavan
BEA139 Dhruv Mulay
BEA145 Ismail Shaikh

1. Install Nodejs(LTS) on the local machine.

2. After installing NodeJS install hardhat using npm. The command for installing Hardhat using npm is 'npm install hardhat'.

3. Extract the zip folder provided and open the extracted folder in Visual Studio Code or anyof your favourite code editor.

4. Open the extracted folder in Code editor. Open the termianl in the folder and execute command 'npm install' follwed by 'npx hardhat node'.

5. Open browser and setup metamask wallet.

6. Setup the Hardhat network by clicking on Settings -> Network -> Add a network -> Add a network manually (at bottom).

7. The details for Hardhat network are

	Network Name: Hardhat
	
	New RPC URL: http://127.0.0.1:8545/

	Chain ID: 1337
	
	Currency symbol: HardhatETH

8. After saving this hardhat network , switch to hard hardhat network.

9. We need to to import some account with test ethers in the metamask wallet. Open the terminal on which hardhat server is running i.e. on which 'npx hardhat node' is running'.

10. There is a list of 20 account with 10000 ETH each that can be used for development purpose. Account address along with the privte key will be given.

11. Copy the private key given with the account. 

12. Open Metamask extension and click on account drop down -> + Add Account or Hardware wallet -> Import account -> Paste the account's provate key whcih is copied -> click on import. The account has been successfully imported.

13. Import a few wallets that as we require a few wallets for demonstration of this project.

14. Open a new terminal in the project directory which is extracted and execute command 'npx hardhat run --network localhost scripts/deploy.js'. 

    This will deploy the smart contract on your running Hardhat server. NOTE: For this 'npm hardhat node' must be running on other terminal.

15. After the contract is deployed, contract address will be provided like 'Library deployed to: 0x5FbDB2315678afecb367f032d93F642f64180aa3'. Copy the value.

16. Open App.js file. client -> src -> App.js. On line no. 30 there is there is 'let contractAddress = "0x5FbDB2315678afecb367f032d93F642f64180aa3"' paste your copied contract address in already present contract address value.

17. Open a new Terminal in the project folder. (NOTE: 'npx hardhat node' must me running for the entire timeline of the project). cd into the client folder.

18. Exectute the command 'npm install' followed by 'npm start' inorder to start the react project.

19. After this the react project will get opened on 'http://localhost:3000' , if it is not opened automatically then paste the url in the browser.

20. After this you can access Add data, get data, share data, etc as well as you can change the account through metamask.


In above steps we have successfully setup and executed the 'Block Storage' project which uses hardhat, ReactJS and Metamask.