# User Stories

**Make a Deposit**

As a user, Alice would like some credits for a given wallet.  She obtains a deposit address, then sends a deposit to that address.  The funds should show up in the CreditChain, and consequently, the Ledger after the transfer is confirmed.

**Paint a pixel on Lightning Testnet**

Bob wishes to paint a pixel on the website, [testnet.satoshis.place](https://testnet.satoshis.place/), however does not have a testnet lightning wallet.  Bob acquires some funds on solid from a friend and then decides which pixel to paint.  And invoice is created and the pixel is painted.  Bob's balance is reduced by one satoshi and recorded in the CreditChain.

**IPFS Pinning**

The IPFS system is used to store content addressable files.  Peers can 'pin' a file making it globally accessible.  However there is a cost associated with that.  Micro payments could incentivize a user to pin a file and receive an income.

**Pay for Hosting**

It may be possible to use the system to pay for the hosting of your wallet or other files with micro payments themselves.  In this way you can get a a bit of storage space and be confident your files will be long lived.

**Faucet**

A faucet is a simple tool to get users started with a bit of currency.  It can be used to test or to buy services to help those with less funds.

**Paywall**

A pay wall is an access controlled piece of content.  Sending a micro payment to the right place can open up the content.  Solid is well suited to such use cases with its ACL system.

**Dynamic DNS Service**

Dynamic DNS allows you to use a name server to root traffic to your own computer.  It's useful but often a pay service.  Micro payments could allow you to use a name server in order to share files on your laptop, desktop or other device.

**Smart Proxies**

Proxies can be used to get files such as a CORS proxy for javascript.  However you may want to throttle how much a given user can take, micro payments could allow a set limit on your proxy.

**Make a Withdrawal**

Withdrawals can be orchestrated by someone in the system with a balance.  It is a bad idea to store any funds on a server, as it invites hackers.  A hot wallet may be a solution but suffers from the same limitation.  A better solution might be have withdrawal requests sent to trusted notaries who verify the size and the request, then process based on cold storage, or a hardware wallet.

