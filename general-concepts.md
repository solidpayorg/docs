# General Concepts

## **Wallet**

![A Test Wallet](.gitbook/assets/testwallet.png)

A **Wallet** is the parent of a _Ledger_ and a set of transactions, which is known as the _CreditChain_.  It can have meta data associated with it.  By convention every Wallet will have exactly one currency that is used throughout the system.

## **Ledger**

![A Test Ledger](.gitbook/assets/testledger.png)

A **Ledger** is a set of users and balances.  Every user is denoted using a URI.  A Wallet will also have a start state.  Also known as the Genesis Ledger.  By default all balances are null in the Genesis Ledger.  The Ledger is a derived data structure that is calculated from the start state and using the _CreditChain_.

## **CreditChain**

![A Test CreditChain](.gitbook/assets/testcreditchain.png)

A **CreditChain** is a chain of credit transactions that is used to derive the _Ledger_ from the initial state.  _Credits_ are ordered and collected together so that the _Ledger_ can be verified and computed.

### **Credit / Transaction**

A **Credit** is a web credit that indicates a payment between two counter parties.  Another name for a Credit is a Transaction, the two terms will be used interchangeably.  By default the rule is that you cant send more funds that you have.  In other words no balance can drop below zero.

### Deposit

A **Deposit** is a special kind of _Transaction_ that comes from an external system of the same currency.  For example you could deposit from a bitcoin testnet address to the address of a URI.  On verification of that transaction the URI can receive a higher balance.

### **Coinbase**

A **Coinbase** is a special optional account in the Genesis Ledger which is allowed to start above zero.  The wallet creator will typically control the Coinbase and set the rules of emission ie how those coins are distributed to the user base.  A Coinbase will normally be backed by goods, services or other assets.

## Inbox

An **Inbox** is a useful mechanism advertised by a wallet which instructs an agent where to send new _Credits_.  Typically, those credits will be validated on receipt and if valid added immediately to the _CreditChain_, with the _Ledger_ updated.

