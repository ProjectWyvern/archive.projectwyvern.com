---
layout:       single
title:        "Wyvern Exchange Beta"
date:         2017-11-03 00:00:00 -0400
categories:   Exchange
---

### What is the Wyvern Exchange?

#### Basics

The Wyvern Exchange is an automated distributed marketplace where users can buy and sell any kind of digital item: game keys, skin codes, promotion redemption instructions, etcetera. Items can be bought and payed for instantly using the Wyvern cryptocurrency.

#### Sale Methods

Items can be sold at a fixed price, in bulk if desired, or alternatively in a fixed-time variable-price auction, where the seller sets a deadline and the highest bid by the deadline wins the item. Bids will require an Ethereum transaction (with some token gas cost) to deter spam.

### Development Timeline

The Wyvern Exchange is in active development; [check out the landing page][landingpage] periodically (or sign up there with your email address for Wyvern Exchange-related updates).

Expect a testable beta version (fake currency but otherwise real functionality) within a week or so.

### Initial Architecture

*N.B. We're committed to choosing the best possible backend architecture for Wyvern Exchange users. As underlying dApp capabilities evolve, we'll update our model, but initially the Wyvern Exchange will work roughly as following.*

#### ERC20 Two-Way Peg

Ethereum, despite some architectural shortcomings, is currently the only production-ready smart contract platform and will be used for the initial Wyvern Exchange dApp. The existing Wyvern chain will be two-way pegged to an ERC20 token (watch in the next few days for further discussion of this mechanism), so users can convert original-chain Wyvern into ERC20 Wyvern and vice versa. Tokenized ERC20 Wyvern will be used to pay for virtual merchandise on the exchange, and will be usable anywhere standard ERC20 tokens are (e.g. on Etherdelta). 

#### Wyvern Exchange Smart Contract

The Wyvern Exchange smart contract will maintain a user account registry, allow users to deposit and withdraw ERC20 Wyvern, track user balances, and handle merchandise sale transactions trustlessly (so you need not trust the operators of the Wyvern Exchange to hold your funds).

#### Community-Arbitrated Escrow System

Purchasers of items on the Wyvern Exchange may optionally, for a small fee, request that their payment be escrowed. If they do so, once they purchase an item, the Wyvern Exchange smart contract will hold funds until the buyer verifies the validity of the purchased item and releases escrow. If the buyer disputes the validity and wishes to reclaim their funds, they may open an escrow dispute case. Dispute cases will be resolved by majority vote of an arbitration board composed of trusted Wyvern Exchange users, who will each receive a portion of the escrow fee in compensation for their time.


[landingpage]: https://exchange.projectwyvern.com
