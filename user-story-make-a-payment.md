# User Story : Make a Payment

### User Story

As a user, Alice wishes to pay Bob, 10 units for a pizza. She creates a web credit, and adds a note of "Pizza". This is then sent to the wallet inbox, and Bob's balance is increased.

### Process <a id="process"></a>

Alice creates a web credit with source Alice, and destination Bob \(both URIs\).  She sets the amount to 10 and the currency to the wallet currency.  She sets the description to "Pizza".  After adding a timestamp and id, she sends the web credit to the wallet inbox.  The wallet processes the credit, and if valid, updates the credit chain and changes the ledger.

### File Based Credit Chain

Validation first verifies that the credit was sent by the user.  This can be done via digital signatures, or in the login handshake.  Next the fields must be well formed.  [ShEx](https://www.w3.org/2001/sw/wiki/ShEx) for example can be used here.  Finally the user must have enough funds for the credit.

If the credit validates, it is added to the CreditChain.  The simplest implementation uses flat files for each block in the credit chain.  Given that files cannot grow indefinitely in length, it may be practical to set a max number of credits per file, and link to the previous.  Atomically the Ledger is also incremented and decremented based on the credit.

### Timestamps

The order of the credits is important, in order to guarantee the integrity of the ledger.  Time stamps can often drift in global systems, or clocks can be incorrect.  In such a way the credits may require next / prev pointers in order to preserver order, or in built ordering structures such as arrays or lists.  This relates to the subtle distinction between time and block chains.

### Comments

It is optionally possible to add a comment to a payment.  There is a desired social effect around tipping \(aka marking\) in order to reward users who have behaved well and to leave a short reason why that payment was made.  This can lead to a contextual web of reputation encouraging good behaviour, discouraging bad behaviour and creating a metric.

