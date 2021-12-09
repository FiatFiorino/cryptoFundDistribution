## Crypto/Token Distribution Script

This Smart contract has been designed to allow for the distribution of polygon tokens 
(MATIC) to multiple wallets.

###### How it works
The contract needs to be compiled in an IDE, I use Remix (https://remix.ethereum.org/)
Import the file tokenFundDistribution (or cut and paste the code).

For use on the Polygon TestNet (https://mumbai.polygonscan.com/) I compiled the smart 
contract using the compiler build v0.4.11+commit.68ef5810.

I did not enable optimization and left the number of runs at the default of 200.

The smart contract compiles with no errors.

Once compiled it needs to be pushed to the TestNet.

This is completed using the "Deploy and Run Transactions" tab within the ReMix IDE.
The contract to be depolyed is called "RKPRIM - <yourfilename.sol>" I deployed it using
Injected Web 3 (MetaMask). You'll need to add the Mumbai Polygon TestNet to MetaMask 
before deploying the smart contract. 
(https://docs.polygon.technology/docs/develop/metamask/config-polygon-on-metamask/)

Once deployed to the Mumbai TestNet the contract will need to be configured for 
distribution.

Step One:
verify the smart contract on the TestNet.

Step Two:
lock the smart contract to the same wallet that published it. This is done via the lock
button/function on the smart contract "write" page. You will be asked to sign this 
transaction using MetaMask.

Step Three:
Now it's time so set up the distribution of the tokens based upon percentages. This
smart contract uses the following logic 1% = 10.

  For Example
  If I wanted to send 15% to Wallet A, 25% to Wallet B and the remaining 60% to 
  Wallet C, I would do the following;
  
  Using the "write contract" page, scroll down to "addAccount"
  Enter the public key of Wallet A in the * _addr (address)* field,
  150 in the *_pctx10 (uint256)* field and
  



---

The compiler v0.4.11+commit.68ef5810 has the following known specific version warnings:

The compiled contract might be susceptible to EmptyByteArrayCopy (medium-severity), 
DynamicArrayCleanup (medium-severity), 
ImplicitConstructorCallvalueCheck (very low-severity), 
TupleAssignmentMultiStackSlotComponents (very low-severity), MemoryArrayCreationOverflow 
(low-severity), privateCanBeOverridden (low-severity), SignedArrayStorageCopy 
(low/medium-severity), UninitializedFunctionPointerInConstructor_0.4.x 
(very low-severity), IncorrectEventSignatureInLibraries_0.4.x (very low-severity), 
ExpExponentCleanup (medium/high-severity), NestedArrayFunctionCallDecoder 
(medium-severity), ZeroFunctionSelector (very low-severity), DelegateCallReturnValue 
(low-severity), ECRecoverMalformedInput (medium-severity), SkipEmptyStringLiteral 
(low-severity) Solidity Compiler Bugs.


