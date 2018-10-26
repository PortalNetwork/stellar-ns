![Stellar Name Service](./assets/title.jpg)

> 📖🔍 Documents of the Stellar Name Service.

# Overview

## 💡 What is Stellar?
Stellar also known as Stellar Lumen, is a pragmatic blockchain project that aims to function as a bridge between the opposing worlds of cryptocurrency and traditional centralized financial institutions.

## 💡 What is BNS?
BNS – or blockchain name system – is the protocol on the internet that turns human-comprehensible decentralized website names such as 'website.xlm' or 'mywebsite.xlm' into addresses understandable by decentralized network machines.

## 📝 Description
SNS is the Stellar Name Service, a distributed, open, and extensible naming system based on the Stellar blockchain. 

## 📚 Documents

#### Table of Contents
- [Introduction](./docs/INTRODUCTION.md)

## ⌨️ Stellar Development
- [Support Languages](https://www.stellar.org/developers/reference/)
    - [Go](https://www.stellar.org/developers/go/reference/index.html)
    - [Java](https://github.com/stellar/java-stellar-sdk)
    - [JavaScript](https://www.stellar.org/developers/js-stellar-sdk/reference/index.html)
- [REST APIs](https://www.stellar.org/developers/horizon/reference/index.html)
- [Stellar Smart Contract](https://www.stellar.org/developers/guides/walkthroughs/stellar-smart-contracts.html)

## Stellar in Web3.0
Stellar plays an connecting and entry layer in Web3.0 services. It connects with Stellar wallet, bridge server, compliance server, federation server, horizon and stellar blockchain.
![Web3](./assets/web3-stellar.png)

## Stellar Tech Stack

# Introduce

## Bridge Server
Stellar.org maintains a bridge server, which makes it easier to use the federation and compliance servers to send and receive payments. When using the bridge server, the only code you need to write is a private service to receive payment notifications and respond to regulatory checks from the bridge and compliance servers.

## Federation Server
The Stellar federation protocol allows convert a human-readable address like `amy*your_org.com` to an account ID. It also includes information about what should be in a transaction’s `memo`. When sending a payment, you contact a federation server first to determine what Stellar account ID to pay. Luckily, the bridge server does this for you.

## Compliance Server
The task of an anchor is handling regulatory compliance, like Anti-Money Laundering (AML). To accomplish that, you should use the Stellar compliance protocol, a standard way to exchange compliance information and pre-approve a transaction with another financial institution.

You can write your own server that matches the compliance protocol, but Stellar.org also provides a compliance server that takes care of most of the work for you.

Your bridge server contacts your compliance server in order to authorize a transaction before sending it. Your compliance server uses the compliance protocol to clear the transaction with the recipient’s compliance server, then lets the bridge server know the transaction is ok to send.

## Horizon
Horizon is the client-facing API server for the Stellar ecosystem. It acts as the interface between Stellar Core and applications that want to access the Stellar network. Horizon allows you to submit transactions to the network, check the status of accounts, and subscribe to event streams. For more details, see an overview of the Stellar network.

## Stellar Testnet

## Stellar Wallet

## 🔗 Resources
- [Official Website](https://www.stellar.org/)

## 📣 Contributing
See [CONTRIBUTING.md](./CONTRIBUTING.md) for how to help out.

## 🗒 Licence
See [LICENSE](./LICENSE) for details.
