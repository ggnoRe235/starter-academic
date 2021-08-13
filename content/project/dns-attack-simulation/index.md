---
title: DNS attack simulation
date: 2021-03-08T08:12:00.000Z
summary: >-2
    **Apr. 2019 - May. 2019**

  Simulated different methods of DNS attacks and evaluated some approaches that could mitigate these attacks.

    **Attack analysed:**

  * Local DNS server cache poison

  * DNS hijack based on arp spoofing


  **Evaluated approaches:**


  * If local DNS server uses random UDP ports for DNS queries, attackers only have slightly chance(1/(2^48)) to figure out the correct DNS query id and UDP port at the same time, and thus the possibility that the local DNS server will receive false responses from attackers is very small.

  * Instead of using UDP to have DNS queries, DoT(DNS over TLS) and DoH(DNS over Https) can both encrypt DNS queries and the encrypted traffic is mixed with other normal traffic, which makes it difficult for attackers to figure out and analyse users' DNS queries.
draft: false
featured: false
tags:
  - net
  - sec
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
  **Apr. 2019 - May. 2019**

Simulated different methods of DNS attacks and evaluated some approaches that could mitigate these attacks.

  **Attack analysed:**

* Local DNS server cache poison
* DNS hijack based on arp spoofing

**Evaluated approaches:**

* If local DNS server uses random UDP ports for DNS queries, attackers only have slightly chance(1/(2^48)) to figure out the correct DNS query id and UDP port at the same time, and thus the possibility that the local DNS server will receive false responses from attackers is very small.
* Instead of using UDP to have DNS queries, DoT(DNS over TLS) and DoH(DNS over Https) can both encrypt DNS queries and the encrypted traffic is mixed with other normal traffic, which makes it difficult for attackers to figure out and analyse users' DNS queries.
