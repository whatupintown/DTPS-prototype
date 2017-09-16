# 1. DTPS prototype
Solidity smart contract that can demo the simplest ticket pre-sale:
- Defines one ticket with a dedicated price in $ETH.
- Defines the funding goal (how many tickets need to be sold to make the event happen).
- Defines a deadline for the fund raising.
- Defines a recipient wallet address.

Ticket reservation takes place by sending ticket price in $ETH + execution fee to the contract. At the time of the deadline or later the contract can be executed to do one of the following two things: 

1) If the funding goal has been reached the locked up funds are sent to the recipient address. The owner of that wallet can execute a function that returns a list of all wallet addresses that have purchased a ticket. 

2) If the funding goal has not been reached all wallet addresses that have reserved a ticket receive their funds back.
