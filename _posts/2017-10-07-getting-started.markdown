---
layout:       single
title:        "Getting Started with Wyvern"
date:         2017-10-07 00:00:00 -0400
categories:   Tutorials
---

### Choose Your Wallet

#### Windows / Mac OS X / Linux

See [the repository][github] for instructions.

Continuous-integration binaries will be provided ASAP.

#### Docker

An [officially maintained Docker image][docker] is autobuilt from the Wyvern source repository.

If you have Docker, launching a Wyvern node will take only a minute:

{% highlight bash %}
$ mkdir ~/.wyvern
$ echo 'rpcuser=xyz\nrpcpassword=xyz' > ~/.wyvern/wyvern.conf
$ docker run -d -v ~/.wyvern:/root/.wyvern --name wyvern protinam/wyvern /root/wyvern/src/wyvernd
{% endhighlight %}

Once you've launched the image, run commands through Docker:

{% highlight bash %}
$ docker exec wyvern /root/wyvern/src/wyvernd getinfo
{% endhighlight %}

### Acquire some Wyvern

An official faucet is soon-to-come. For now, the easiest way to acquire Wyvern is by mining some at a pool or buying some at an exchange - examine your options at [Service Providers][serviceproviders].

[github]:           https://github.com/protinam/wyvern
[serviceproviders]: /general/service-providers/
[docker]:           https://hub.docker.com/r/protinam/wyvern/
