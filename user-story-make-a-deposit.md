# User Story : Make a Deposit

### User Story

As a user, Alice would like to add some credits for a given wallet.  She obtains a deposit address, then makes a deposit to that address.  The funds should show up in the CreditChain, and consequently, the Ledger, after the transfer is confirmed.

### Process

In Solid Pay every user is denoted by a URI.  In order to make a deposit from an external system, there needs to be a one to one relationship between the deposit address and that URI.  Once the deposit is observed in the external system, a new web credit can be created which references the external transaction.  The source will be defined as the external sender of that transaction.

### Deposits from Bitcoin and Bitcoin Testnet

The method described here uses [Hierarchical Deterministic Wallets](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki) \(HD Wallet\).  This has the advantage of ensuring that funds never live on the server, leading to better security.  A keypair is generated and the public key is added to the wallet definition.  From this public key, it is possible to derive a child public key for any hashed URI.

Code to do this can be seen [here](https://github.com/quantumpayments/hdwallet/blob/master/test/util.js).  The private key is kept in cold storage and only used when withdrawals are to be made.

When making a deposit from the other network to the solid pay wallet, you need only include the source address, the paid to \(derived\) URI address, and a hint in the description showing the transaction ID in the bitcoin network.  The system is then pinged in order to verify the transaction occurred, and the new web credit is generated.

Deposits are linked closely with withdrawals.



