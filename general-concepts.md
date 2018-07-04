# General Concepts

**Wallet**

A wallet is the parent of a ledger and a set of transactions.  It can have meta data associated with it.  By convention every wallet will have exactly one currency that is used throughout the system.

**Ledger**

A ledger is a set of users and balances.  A ledger will also have a start state.  Also known as the Genesis Ledger.  By default all balances are null in the Genesis Ledger.

**Credit / Transaction**

A credit is a web credit that indicates a payment between two counter parties.  Another name for a credit is a transaction, the two terms will be used interchangeably.  By default the rule is that you cant send more funds that you have.  In other words no balance can drop below zero.

**CreditChain**

A credit chain is a chain of credit transactions that create the ledger from the initial state.

**Coinbase**

A coinbase is a special account in the Genesis Ledger which starts above zero.  The wallet creator will typically control the coinbase and set the rules of emission ie how those coins are distributed to the user base.  A coinbase will normally be backed by goods, services or other assets.

