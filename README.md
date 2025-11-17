## Experiment 1: Private Blockchain
## Aim:

To implement a secure passwordless authentication system in PrivateBlock using public–private key cryptography, where users authenticate by signing a challenge instead of using passwords.

## Algorithm
Step 1: 
The user provides their public key to the system. The system stores this key as the user’s identity.

Step 2: 
When the user wants to log in, the system creates a random challenge (nonce) and sends it to the user.

Step 3: 
The user signs the challenge using their private key and sends the signature back to the system.

Step 4: 
The system verifies the signature using the stored public key.
If valid, the user is successfully authenticated.

## Program 
### Genesis file privateblock.json
```
{
"config" {
"chainId" 878787,
"homesteadBlock" 0,
"eip150Block" 0,
"eip155Block" 0,
"eip158Block" 0,
"byzantiumBlock" 0,
"constantinopleBlock" 0,
"petersburgBlock" 0,
"istanbulBlock" 0,
"berlinBlock" 0,
"clique" {
"period" 5,
"epoch" 30000
}
},
"difficulty" "1",
"gasLimit" "8000000",
"extradata"
"0x00000000000000000000000000000000000000000000000000000000000000001d09cd3F475a65
7381b223A9c91029865b27E0270000000000000000000000000000000000000000000000000000000
000000000000000000000000000000000000000000000000000000000000000000000000000",
"alloc" {
"1d09cd3F475a657381b223A9c91029865b27E027" { "balance" "3000000000000000000" },
"e503980FB9E4D17048b973B0ee01759DcF2d7879" { "balance" "3000000000000000000" }
}
}
```
### Smart Contract New.sol
```
//SPDX-License-Identifier MIT
pragma solidity ^0.8.19;
contract New{
string name;
function setName(string memory _name) public {
name= _name;
}
function getName() public view returns (string memory){
return name;
}
}
```
## Output 


## Result
RESULT: Thus, the Private Blockchain is created, nodes are added with accounts, and Ether is transferred into it by creating and deploying Smart contract successfully
