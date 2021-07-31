---
title: An investigation on the security of DNS servers in China
date: 2021-07-31T08:09:11.519Z
summary: >-2
    **Apr. 2019 - May. 2019**

  Analysed 500 DNS servers’ responses towards 20 different domain names with traceroute, nslookup and wireshark.

    **Brief introduction:**

  * This research tests 500 DNS servers provided by Hunan university, google, and different ISPs in China. The 20 tested domain names include 15 common domain names in China, 3 domain names of google and 2 inexistent domain names. By analysing these DNS servers’ reply, a series of DNS security problems has been found.


  **Conclusion:**


  * Different ISPs in China have different strategies toward inexistent domain names. DNS server provided by China Mobile will direct user to its ads page if requested domain name doesn’t exist while other ISPs won’t.

  * DNS servers provided by university can resolve all domain names correctly, while all DNS servers provided by ISPs will give false replies toward domain names of google.

  * When user assign ”8.8.8.8” as its DNS server and request domain names of google, ISPs will analyse user’s requests and reply a false IP before the real DNS server
draft: false
featured: false
tags:
  - sec
  - net
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
  **Apr. 2019 - May. 2019**

Analysed 500 DNS servers’ responses towards 20 different domain names with traceroute, nslookup and wireshark.

  **Brief introduction:**

* This research tests 500 DNS servers provided by Hunan university, google, and different ISPs in China. The 20 tested domain names include 15 common domain names in China, 3 domain names of google and 2 inexistent domain names. By analysing these DNS servers’ reply, a series of DNS security problems has been found.

**Conclusion:**

* Different ISPs in China have different strategies toward inexistent domain names. DNS server provided by China Mobile will direct user to its ads page if requested domain name doesn’t exist while other ISPs won’t.
* DNS servers provided by university can resolve all domain names correctly, while all DNS servers provided by ISPs will give false replies toward domain names of google.
* When user assign ”8.8.8.8” as its DNS server and request domain names of google, ISPs will analyse user’s requests and reply a false IP before the real DNS server
