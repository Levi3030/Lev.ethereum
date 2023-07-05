CREATE A TOKEN

This SOLIDITY assessment aims to create an nft token in a simple and easy way in order for newbie students can understand with ease.

## Description

This contract is a basic simulation on how NFTs work and how to create it.

## Getting Started


### Executing program

- First you need to create string variables.
- Use a function called mapping address and make it public.
- Create a mint function that both parameters has an address and uint.
- Create a burn function, it is nearly the same as the mint function but replace the "+" with a "-" and add a if statement.
- Deploy your NFT and try its features.
```

contract MyToken {

    // public variables here
    string public name = "REMIX";
    string public abbrv = "RNB";
    uint public supply = 0;

    // mapping variable here
         mapping(address => uint) public blnc;

    // mint function 
        function mint (address add, uint val) public{
           supply += val;
           blnc [add] += val;
        }

    // burn function
        function burn(address add, uint val) public{
           if(blnc[add] >= val){
              blnc[add] -= val;
           }
        }

}

## Authors

Contributors names and contact info

Johm Vinas  
[Facebook.com/johnlevi30] (https://web.facebook.com/johnlevi30/)


