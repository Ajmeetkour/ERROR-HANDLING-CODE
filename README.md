# Error Handling

This Solidity program is "Error handling" program that demonstrates the error handling concept and functionality of  revert(), assert() and require() statement of the Solidity programming language.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has three function that returns the differnt values . This program serves as a simple and straightforward introduction to Error handling concept in Solidity programming, and can be used as a stepping stone for more complex projects in the future.

## Getting Started

### Executing program

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract PaymentContract {
    uint public GST=200;
  
    function Totalvalue(uint  payment) public view returns(uint) {
        require(payment > 0, "payment must be greater than zero");
        return GST+payment;
    }

    function Donation(uint Salary) public pure {
    
        if (Salary<30000) {
            revert("You can't donate");
        }
    }

    function ConditionVerification(uint donation) public pure {
      
        assert( donation > 500);
    }
}
To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.0" (or another compatible version), and then click on the "Compile Error.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "Error" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling the conditionverification, donation, Totalvalue function. Click on the "Paymentcontract" contract in the left-hand sidebar, and then click on all the functions one by one. Finally, click on the "call" button to execute the function and retrieve the  message.

## Authors

Ajmeet kour


## License

This project is licensed under the MIT License - see the LICENSE.md file for details
