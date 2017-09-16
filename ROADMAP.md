## 1. DTPS prototype
Solidity smart contract that can demo the simplest ticket pre-sale:
- Defines one ticket with a dedicated price in $ETH.
- Defines the funding goal (how many tickets need to be sold to make the event happen).
- Defines a deadline for the ticket pre-sale.
- Defines a recipient wallet address (host).

Ticket reservation takes place by sending ticket price in $ETH to the contract. The contract locks up the funds. At the time of the deadline or later the contract can be executed to do one of the following two things:

a) If the funding goal has been reached the locked funds are sent to the recipient address (host). The owner of that wallet can execute a function that returns a list of all wallet addresses that have purchased a ticket. Later this list can be used to handle check-in at the event.

b) If the funding goal has not been reached all wallet addresses that have reserved a ticket receive their funds back (later on it will be possible to specify a different cash back address).

## 2. DTPS alpha
Integrates all sorts of features to make the prototype usable in real life. 

## 3. DTPS beta
Contract security and tests.

## 4. Python API to access the contract
TBD...

## 5. Integration of Shapeshift and/or Changelly to support payments with other cryptocurrencies
TBD...

## 6. Python DTPS generator (package) to configure, generate and deploy DTPS contracts
TBD...

## 7. Integration of a fiat payment solution
TBD...

## 8. Javascript API to access the contract
TBD...

## 9. Javascript DTPS generator (package) to configure, generate and deploy DTPS contract
TBD...
