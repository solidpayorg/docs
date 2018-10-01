# Appendix A : Sample Data

### Wallet in turtle

```text
@prefix : <https://w3id.org/cc#> .

<#this> a :Wallet .
<#this> <http://purl.org/dc/terms/description> """Test Wallet for the Solid economy""" .
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

### Credit and CreditChain in turtle

```text
@prefix : <https://w3id.org/cc#> .

<> a :CreditChain .
<>  <http://www.w3.org/2000/01/rdf-schema#label> "Solid Test Credit Chain" .

<https://melvin.solid.live/profile/card#me> <http://www.w3.org/2000/01/rdf-schema#label> "Melvin Carvalho OIDC" .

<https://melvincarvalho.com/#me> <http://www.w3.org/2000/01/rdf-schema#label> "Melvin Carvalho TLS" .
<https://www.w3.org/People/Berners-Lee/card#i> <http://www.w3.org/2000/01/rdf-schema#label> "TimBL" .
<mailto:eric@w3.org> <http://www.w3.org/2000/01/rdf-schema#label> "Eric Email" .


<#1>  a <https://w3id.org/cc#Credit> ;  
<https://w3id.org/cc#source> <bitcoin:mwni7TwyvJTUVadTUXPaVvZ29cRbd9gaXB> ; 
<https://w3id.org/cc#destination> <https://melvincarvalho.com/#me> ;   
<https://w3id.org/cc#wallet> <https://melvin.solid.live/public/appdata/ledger/testwallet.ttl> ;   
<https://w3id.org/cc#amount> 10 ;  
<https://w3id.org/cc#description> "0db9a2e63a8ddc57db1355ca1606c3f1d7fc9684cc55ff255b3bdc2c55e2d470" ;  
<https://w3id.org/cc#currency> <https://w3id.org/cc#testMBTC> .


<#2>  a <https://w3id.org/cc#Credit> ;  
<https://w3id.org/cc#source> <https://melvincarvalho.com/#me> ; 
<https://w3id.org/cc#destination> <https://melvin.solid.live/profile/card#me> ;   
<https://w3id.org/cc#wallet> <https://melvin.solid.live/public/appdata/ledger/testwallet.ttl> ;   
<https://w3id.org/cc#amount> 1 ;  
<https://w3id.org/cc#currency> <https://w3id.org/cc#testMBTC> .

<../testwallet.ttl#this> a :Wallet .
<../testwallet.ttl#this>  <http://www.w3.org/2000/01/rdf-schema#label> "Solid Test Wallet" .
<../testwallet.ttl#this> :currency :testMBTC .
<../testwallet.ttl#this> :ledger <../ledger/ledger.ttl> .
<../testwallet.ttl#this> :creditChain <../credits/creditChain.ttl> .
```

