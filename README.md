# Crypto/Token Distribution Script

This Smart contract has been designed to allow for the distribution of polygon tokens 
(MATIC) to multiple wallets.

# How it works
The contract needs to be compiled in an IDE, I use Remix (https://remix.ethereum.org/)
Import the file tokenFundDistribution (or cut and paste the code).

For use on the Polygon TestNet (https://mumbai.polygonscan.com/) I compiled the smart 
contract using the compiler build v0.4.11+commit.68ef5810.

I did not enable optimization and left the number of runs at the default of 200.

The smart contract compiles with no errors.

Once compiled it needs to be pushed to the TestNet.

This is completed using the "Deploy and Run Transactions" tab within the ReMix IDE



---------------------------------------------------------------------------------------
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
---------------------------------------------------------------------------------------
