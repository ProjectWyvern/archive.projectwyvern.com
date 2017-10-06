---
layout:       single
title:        "Development Guide"
date:         2017-10-07 00:00:00 -0400
categories:   Tutorials
---

### Dependency Installation


For Debian/Ubuntu:

{% highlight bash %}
# apt-get update && apt-get -y install qt5-default \
    qt5-qmake qtbase5-dev-tools qttools5-dev-tools \
    build-essential libboost-dev libboost-system-dev \
    libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev \
    libssl-dev libdb++-dev libminiupnpc-dev
{% endhighlight %}

### Clone the Repository


{% highlight bash %}
# git clone https://github.com/protinam/wyvern.git
# cd wyvern
{% endhighlight %}

### Build Wyvern


To build the core daemon (wyvernd):

{% highlight bash %}
# cd src && make -f makefile.unix -j $(nproc)
{% endhighlight %}

To additionally build the GUI wallet, from the root directory:

{% highlight bash %}
# qmake && make -j $(nproc)
{% endhighlight %}

Make changes, rebuild, test, and repeat as necessary.
