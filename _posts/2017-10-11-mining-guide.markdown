---
layout:       single
title:        "Mining Guide"
date:         2017-10-11 00:00:00 -0400
categories:   Tutorials
---

Wyvern uses a hybrid PoW/PoS consensus algorithm (see [Technical Overview][overview]), using the NIST5 algorithm for proof-of-work.

If you want to mine Wyvern using proof-of-work, you'll need to select appropriate mining software for your hardware and choose whether you want to mine solo or mine with a pool.

## Mining Software

### Nvidia GPUs

[CCminer][ccminer]

### AMD GPUs

[SGminer][sgminer]

### CPUs

[cpuminer-multi][cpuminer-multi]

## Pools

### Hosted

See [Service Providers][serviceproviders] for hosted pools.

### Solo

[Wyvern Solo Pool][solopool]

[overview]:         /general/technical-overview
[ccminer]:          https://github.com/tpruvot/ccminer/releases
[sgminer]:          http://cryptomining-blog.com/2779-new-sph-sgminer-nist5mod-with-higher-performance-for-talkcoin-mining/
[cpuminer-multi]:   https://github.com/tpruvot/cpuminer-multi
[serviceproviders]: /general/service-providers
[solopool]:         https://github.com/protinam/wyvern-solo-pool
