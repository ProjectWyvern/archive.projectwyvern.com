---
layout:       single
title:        "Development Plans"
date:         2017-10-07 00:00:00 -0400
categories:   General
---

### Wyvern Exchange

The Wyvern Exchange, currently under development, will allow users to buy and sell virtual goods using Wyvern. Architecture to-be-determined; possibly a DApp. We're currently looking for frontend developers / designers - if you're interested, [get in touch][contactus]!

### Core

#### Immediate Roadmap

##### Modernize Codebase

The original Wyvern codebase is based on a version of the Bitcoin Core source that's now several years out of date - first up on the development docket is modernization of Wyvern by rebasing on a newer Bitcoin release version. This will bring speed improvments, increased ecosystem compatibility, and a better future upgrade path.

##### PoS Changes

Wyvern utilizes a hybrid PoW/PoS algorithm which may be vulnerable (once the PoW phase is complete) to nothing-at-stake attacks. Before that time, research should be done into alternative proof-of-stake algorithms which do not suffer from this vulnerability, and Wyvern should switch to such an algorithm (this shouldn't require changing any emission parameters).

#### Possible Future Plans

In order to provide utility to the cryptocurrency development space in general, and to provide a unique value proposition for the coin itself, I think Wyvern should pursue one or multiple specific verticals in developmental direction that have not yet been explored. I have a few ideas, but I'm also open to suggestions.

These should not be considered commitments; much further research remains to be done.

##### Value pool-based zkSNARK anonymity

Zcash implements zkSNARKs to provide privacy-preserving transactions, but does so in a way which requires any user of Zcash, regardless of whether or not they use z-addresses / shielded transactions, to trust the integrity of the trusted setup - if the trusted setup were to have been compromised, the party which compromised it could mint unlimited Zcash without ever being detected (or caught - the "fake" Zcash would not be traceable).

A conceivable alternative implementation, as alluded to in the "Privacy" section of the Tezos overview paper (probably among other sources), would be to have two "kinds" of the asset, in this case Wyvern, shielded and unshielded. Unshielded Wyvern could be transacted as normal, publically. Shielded Wyvern could be transacted privately using zkSNARK-proofs. Shielded and unshielded Wyvern could be converted to and from one another - however, the total amount of conversion would be tracked to ensure that no more unshielded Wyvern could be created than was previously shielded. Thus, users of unshielded Wyvern would not be vulnerable to fake Wyvern created by a party which compromised the trusted setup.

Additionally in this vein, I think there is room for quite a bit of innovation with trusted setups - for example, writing a setup in such a way as to support a higher number of participants, or even putting part of the setup itself on-chain.

[contactus]: /general/contact-us
