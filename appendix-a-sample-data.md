# Appendix A : Sample Data

### Wallet in turtle

```text
@prefix : <https://w3id.org/cc#> .

<#this> a :Wallet .
<#this> <http://purl.org/dc/terms/descriptoin> """Test Wallet for the Solid economy""" .
<#this>  <http://www.w3.org/2000/01/rdf-schema#label> "Solid Test Wallet" .
<#this> :ledger <./ledger/ledger.ttl> .
<#this> :currency :testMBTC .
<#this> :inbox <./inbox> .
<#this> :creditChain <./credits/creditChain.ttl> .
<#this> :HDPubKey "xpub661MyMwAqRbcG7Cah2MEx8VkzJ2vWMBGciqTgXYEY6hx4CHLrB6Rf7iQvM4nMm7d2JNV3bVKeKLsbNBMt4fcBFjUnNs63KBRrG4e7oJ47YR" .

```

### Ledger in turtle

```text
@prefix : <https://w3id.org/cc#> .

<> a :Ledger .
<>  <http://www.w3.org/2000/01/rdf-schema#label> "Solid Test Ledger" .

<https://melvincarvalho.com/#me> :amount 9 .
<https://melvin.solid.live/profile/card#me> :amount 1 .

<https://melvin.solid.live/profile/card#me> <http://www.w3.org/2000/01/rdf-schema#label> "Melvin Carvalho OIDC" .

<https://melvincarvalho.com/#me> <http://www.w3.org/2000/01/rdf-schema#label> "Melvin Carvalho TLS" .


<../testwallet.ttl#this> a :Wallet .
<../testwallet.ttl#this>  <http://www.w3.org/2000/01/rdf-schema#label> "Solid Test Wallet" .
<../testwallet.ttl#this> :currency :testMBTC .
<../testwallet.ttl#this> :ledger <../ledger/ledger.ttl> .
<../testwallet.ttl#this> :creditChain <../credits/creditChain.ttl> .

```

