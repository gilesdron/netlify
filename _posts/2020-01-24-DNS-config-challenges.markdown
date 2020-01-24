---
layout: post
title:  "Two major challenges around DNS configuration for less-technical internet end-users."
---

In my experience, the biggest two challenges have always been losing MX (mail) records on transfer and understanding TTLs.  

For example, if a customer chooses (or has been instructed) to move the DNS they generally are only directed to update the host (@) and www A records. Which once propagated this results in no mail service until the necessary A, MX and other TXT records such as DKIM, SPF, for example, have been added to the new SOA.  

The other issue is how long these changes take. Many DNS hosts are now raising their TTLs and may not force a reload upon change. Ideally, customers should always lower the TTLs before making any changes to ensure any necessary rollbacks are within minutes rather than hours.  

[Back to home page](https://practical-galileo-423fde.netlify.com/)