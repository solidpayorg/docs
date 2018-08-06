# User Story : Make a Deposit

### User Story

As a user, Alice would like some credits for a given wallet.  She obtains a deposit address, then sends a deposit to that address.  The funds should show up in the CreditChain, and consequently, the Ledger after the transfer is confirmed.

### Process

In Solid Pay every user is denoted by a URI.  In order to make a deposit from an external system, there needs to be a one to one relationship between the deposit address and that URI.  Once the deposit is observed in the external system, a new web credit can be created which references the external transaction.  The source will be defined as the external sender of that transaction.

### Deposits from Bitcoin and Bitcoin Testnet

The method described here uses Hierarchical Deterministic wallets \(HD Wallet\).  This has the advantage of ensuring that funds never live on the server, leading to better security.



