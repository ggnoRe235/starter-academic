---
title: An investigation on the security of DNS servers in China
date: 2021-03-08T08:24:11.519Z
summary: >-2
    **Apr. 2019 - May. 2019**

  Analysed 500 DNS servers’ responses towards 20 different domain names with traceroute, nslookup and wireshark.

    **Brief introduction:**

  * This research tests 500 DNS servers provided by Hunan university, google, and different ISPs in China. The 20 tested domain names include 15 common domain names in China, 3 domain names of google and 2 inexistent domain names. By analysing these DNS servers’ reply, a series of DNS security problems has been found.


  **Conclusion:**


  * Different ISPs in China have different strategies toward inexistent domain names. DNS server provided by China Mobile will direct user to its ads page if requested domain name doesn’t exist while other ISPs will not.

  * ISPs used to use DNS hijack to direct users to a new website with iframe that contains the original page to feed ads, which has become rare, possibly due to the wide use of content security policy and X-Frame-Options.

  * A small amount(3 out of 28) of DNS servers provided by China railway telcom and DNS servers provided by Hunan university can resolve all domain names correctly, while all DNS servers provided by other ISPs will give false replies toward domain names of google.

  * When users assign ”8.8.8.8” as their DNS server and query domain names of google, ISPs will analyse their requests and reply a false IP before the real DNS server

  * Though DoH(DNS over Https) can stop ISPs from analysing users' queries, due to the small amount of DNS servers that accept DoH, it is still easy for ISPs to ban or substitute these DNS servers.
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

* Different ISPs in China have different strategies toward inexistent domain names. DNS server provided by China Mobile will direct user to its ads page if requested domain name doesn’t exist while other ISPs will not.
* ISPs used to use DNS hijack to direct users to a new website with iframe that contains the original page to feed ads, which has become rare, possibly due to the wide use of content security policy and X-Frame-Options.
* A small amount(3 out of 28) of DNS servers provided by China railway telcom and DNS servers provided by Hunan university can resolve all domain names correctly, while all DNS servers provided by other ISPs will give false replies toward domain names of google.
* When users assign ”8.8.8.8” as their DNS server and query domain names of google, ISPs will analyse their requests and reply a false IP before the real DNS server
* Though DoH(DNS over Https) can stop ISPs from analysing users' queries, due to the small amount of DNS servers that accept DoH, it is still easy for ISPs to ban or substitute these DNS servers.
