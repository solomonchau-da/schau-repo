# CardTrading App
CardTrading is a material management application built in Daml.

### I. Overview 
This project was created by using the `empty-skeleton` template. 

Users can create a Card contract, which includes CardDetails as a field, for more information regarding the card.  Users can they give the Card to someone else, or make a Fake to give to someone.  Account contracts can also be kept.  Users can create an account under a company to keep their valuables.  With an account, one can initiate trading with real currency with others with an Account contract.  


### II. Workflow
  1. company creates an Account contract
  2. alice creates an Account contract
  3. alice creates a Card Contract
  4. alice adds Card into Account contract
  5. alice adds balance to own Account
  6. alice GivesPokemon to bob
  7. bob GivesPokemon to alice
  8. alice GivesFakePokemon to bob
  9. test canWithdraw function
  10. test discountMultiple function
  11. test canBuy function

### III. Functions
canWithdraw: Function that uses if..else statement to check if there are enough funds to be taken out of the balance for an Account contract.  
discountMultiple: Function that uses maps to apply a discount for all specified contracts.
canBuy: Function to check if there is a large enough balance to buy specific cards.  

### III. Compiling & Testing
To compile and test, run the pre-written script in the `Test.daml` under /daml OR run:
```
$ daml start
```

All instances of Happy and Unhappy Path Tests are separately tested.  