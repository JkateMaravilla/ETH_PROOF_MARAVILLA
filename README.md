# ETH-PROOF

# Creating a new token

Using the Solidity
This Solidity represents the "docmcstaffin" token name with the token abbreviation "DMC".
It allows for mint and burn tokens, as well as the querying token balances with the address on it.

# Getting Started 

Excuting the program
To run this program, using the Remix Etheruem. To started the program, go to the Remix website at https://remix.ethereum.org/.
You make a record by clicking and explaning the document symbols on the left sidebar.
The file should be saved with the extension.sol. MyToken.sol)

```javascript
// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

contract MyToken {

    // public variables here
   string public tokenName = "docmcstaffin";
   string public tokenAbbrv = "DMC";
   uint public totalSupply = 0;
   
    // mapping variable here
 mapping (address => uint) public balances;
  
    // mint function
   function mint (address _address,uint _value) public {
      totalSupply += _value;
      balances [_address] += _value;
   }
    // burn function
    function burn (address _address,uint _value) public {
       if (balances[_address] >= _value) {
         totalSupply -= _value;
         balances [_address] -= _value;
       }
   
   }
  
   }
```


# Prequisities
Solidity version must be 0.8.18 or higher.

tokenName: The first string variable addressing the name of token which is the "docmcstaffin"
tokenAbbrv: The second string variable addressing the namme of token contraction "DMC"
totalSupply: The totalSupply is a set of unsigned interger variables that set it to zero

# Mapping
To store token adjustments are stored separately the agreement utilizes the
balances planning factors. 

# Mint Functon 
This mint function can be made a new token and sent using the specific address.

# Burn Function
This burn function is to decreased the token from the balance using the address 

# Authors 
Jephtha Kate A. Maravilla
8210377@ntc.edu.ph

# License 
This project is licensed under the MIT License - see the LICENSE.md file for details
