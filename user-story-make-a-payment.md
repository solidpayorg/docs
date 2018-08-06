# User Story : Make a Payment

### User Story

As a user, Alice wishes to pay Bob, 10 units for a pizza. She creates a web credit, and adds a note of "Pizza". This is then sent to the wallet inbox, and Bob's balance is increased.

### Process {#process}

Alice creates a web credit with source Alice, and destination Bob \(both URIs\).  She sets the amount to 10 and the currency to the wallet currency.  After adding a timestamp and id, she sends the web credit to the wallet inbox.  The wallet processes the credit, and if valid, updates the credit chain and changes the ledger.

