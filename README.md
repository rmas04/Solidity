# MyToken
This Solidity program is a simple "MyToken" that demonstrates the basic syntax and functionality of the Solidity programming language. The purpose of this program is to simulate store details about coins or tokens with mint and burning functions.
# Description
This program is a simple contract written in Solidity this program also have a dual function that can mint and burn token this program also show the token name token abbriv and the token tatal supply and balances.
# Getting Started
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.
Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., MyToken.sol). Copy and paste the following code into the file:

     MyToken {

     string public tokenName = "TIGER";
     string public tokenAbbrv = "TGS";
     uint public totalSupply = 0;

     mapping(address => uint) public balances;

     function mint(address _address, uint _value) public {
      totalSupply += _value;
      balances[_address] += _value;
     }
    function burn(address _address, uint _value) public {
      if (balances[_address] >=_value) {
      totalSupply -= _value;
      balances[_address] -= _value;
     }
    }
    }
To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.4" (or another compatible version), and then click on the "Compile MyToken.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "MyToken" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can see the mint burn functions and show balances, token name token abbrv and total supply. Click the mint function then input the account address to address and add value of the token to mint then transact to execute the mint function. Click in burn function you can do the same in mint to just add value to burn transact to execute the burn function. To check balances just input the account address to balances then click balanaces and lastly to check the name of the token and the abbrv of it just click tokenName and tokenAbbrv.
# Authors
Robee Mar A. Suñiga

61802922@ntc.edu.ph
# License
This project is licensed under the MIT License
