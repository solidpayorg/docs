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

