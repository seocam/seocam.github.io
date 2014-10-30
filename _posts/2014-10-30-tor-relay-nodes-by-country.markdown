---
layout: post
title:  "Tor Relays Nodes by Country"
date:   2014-10-30 06:46:51
comments: true
categories: tor
---

Few days ago I've started to wonder what would be the distribution of Tor relay nodes by country. 

After looking for it I've found the page <http://torstatus.blutmagie.de/>. This page lists all relay nodes but it doesn't give many stats about them (at least I couldn't find).

After a couple minutes I end up with a bash script to mine the information I was looking for:

{% highlight bash %}
curl -s http://torstatus.blutmagie.de/ | \
    LC_ALL=C sed -n 's/^.*img\/flags\/\(.*\)\.gif.*$/\1/p' | \
    sort | uniq -c | sort -k2n -r

1673 us
1332 de
 568 fr
 445 nl
 305 ru
 287 gb
 220 se
 203 ca
 120 ch
 113 cz
  97 jp
  92 at
  76 ro
  74 ua
  62 fi
  53 it
  52 au
  51 pl
  50 dk
  49 no
  43 sg
  38 es
  35 gr
  34 hk
  31 lu
  31 br
  31 bg
  31 be
  29 hu
  27 is
  21 sk
  21 lv
  19 lt
  18 il
  18 ie
  17 md
  16 nz
  15 vn
  14 ar
  11 tr
  11 si
  11 pt
  10 kr
  10 in
  10 ee
   9 tw
   8 za
   8 hr
   6 na
   6 my
   6 mx
   4 th
   4 id
   4 cl
   3 kz
   3 eg
   3 ba
   2 rs
   2 pk
   2 pa
   2 mq
   2 co
   2 a1
   1 ve
   1 uy
   1 sa
   1 qa
   1 ph
   1 pe
   1 mt
   1 mk
   1 ma
   1 lr
   1 li
   1 je
   1 im
   1 cy
   1 cn
{% endhighlight %}

Now I wonder why big countries (like Brazil) have such a small participation in Tor network.
