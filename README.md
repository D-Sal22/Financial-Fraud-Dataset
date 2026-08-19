

## Appendix
## Dataset Column Definitions

Below is a description of each column in the synthetic financial‑fraud dataset:

**step**
A time index representing hours in the simulation.  
Example: step 1 = hour 1, step 2 = hour 2, etc.

**type**
The type of financial transaction.  
Common values include:
- `CASH_IN`
- `CASH_OUT`
- `DEBIT`
- `PAYMENT`
- `TRANSFER`

**amount**
The amount of money transferred in the transaction.

**nameOrig**
The ID of the originating (sender) account.  
This is a random string identifier, not a real name.

**oldbalanceOrg**
The sender’s account balance **before** the transaction.

**newbalanceOrig**
The sender’s account balance **after** the transaction.

**nameDest**
The ID of the destination (receiver) account.  
Also a random identifier.

 **oldbalanceDest**
The receiver’s account balance **before** the transaction.

**newbalanceDest**
The receiver’s account balance **after** the transaction.

**isFraud**
Ground‑truth label indicating whether the transaction was fraudulent.  
- `0` = legitimate  
- `1` = fraud

**isFlaggedFraud**
A naive rule‑based flag that marks transactions as fraud **only if the amount > 200,000**.  
This is intentionally simplistic and usually not useful for 
