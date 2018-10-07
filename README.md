---
description: Version 0.1 draft - work in progress
---

# Solid Pay

![Solid Pay!](.gitbook/assets/solidlogo.png)

**Solid Pay** is about making payments between two people on the Web.  It builds heavily on the [Solid](https://github.com/solid/solid) framework and the [webcredits](https://webcredits.github.io/spec/) specification.

### Instantaneous, zero cost transactions, that scale to millions per second

Solid Pay is not a crypto currency it is a higher layer technology that lives above existing currencies.  However, Solid Pay, itself, is currency agnostic and any currency is usable with it.  

Being a higher layer protocol it is capable of thousands or even millions of transactions per second, instantaneously and at zero cost.  The aim is that this will facilitate new use cases and business models.

### Why not use a block chain?

While block chains are a great technology, solid pay builds on _top_ of existing networks.  For example, the bitcoin block chain is instant but requires around ten minutes for a confirmation, has around 4 transactions per second and has a fee market.  

Layer 2 such as lightning network has a deposit in order to participate and two transactions, one to create a channel and another to tear it down.  It can then can scale micro payments across a network efficiently.  

Higher layers such as Solid Pay can interface with both bitcoin and lightning and offers a web based transaction system which uses lower layers for settlement.  Consider a system like adsense.  You may incur millions of clicks over a year, but only cash out once per month.

### Why Solid?

Solid builds on 30 years of Web research and development.  It has a cutting edge semantic layer with proven scalability, capable of smart contracts, ICOs, web hooks, machine feedback loops and much more.  It is available natively in every browser, so no need to install a wallet.  

Solid is a unique platform for payments -- in no other system can you spontaneously create an economy -- _as a user_ -- you dont need any server side programming experience -- just point and click, on any solid compliant system -- every other payment system out there needs installation, turnkey software, and sysadmin experience -- with solid you can just create and tear down economies as they are needed. Quite revolutionary!

Special features such as access control allow advanced use such as public and private ledgers, or even time, block and side chains.  Additionally, append only inboxes allow a unique and secure way of sending transactions from one server to another.  You can only do this with a full read write web, which solid offers.

### What is the Security Model

Solid uses, digital signatures, which is a bit like signing a check.  This means that I can write something but cannot fake it.  If two people on the web trust each other, they can digitally sign things so that the signer cannot take it back.  

This guarantees that the payer is who they say they are and the amount is valid.  Payments are collected into a ledger and the ledger forms a set of balances.  Both of these can be verified.  This ensures that each payment has an audit trail and the balances in the ledger are accurate.

It is a proven security model with decades of battle hardened industry testing.  All communication is encrypted over the wire, so that it is impossible to eves drop.

### About This Guide

Outlined in this guide are general concepts, user stories and technical details for creating and interacting with payment systems on Solid. 

Anyone with a solid pod or that is a solid user can participate, without needing a wallet, however, it should be backwards compatible with the existing web.

