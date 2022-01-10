---
title: Install monitoring on Nighthawk R7000 router
description: Steps on how I installed NETDATA on my R7000 router flashed with
  DD-WRT firmware
author: Luke B
date: 2020-09-01
tags:
  - left
  - center
  - right
---
# Install NETDATA and DD-WRT firmware

![Image of DD-WRT and Netdata](/static/img/screen-shot-2021-12-22-at-6.43.47-pm.png "DD-WRT and Netdata running")

The reason I installed DD-WRT and Netdata was because the stock router was having issues with dropping wireless connections. 

The first thing that I did was to install DD-WRT. How I did that is following the [DD-WRT](https://wiki.dd-wrt.com/wiki/index.php/Netgear_R7000) guide for my router.

After I had the new firmware installed. Everything seemed to be running a lot better but I wanted some monitoring so I could see what is going on at a glance. That is when I decided to try [Netdata](https://www.netdata.cloud/).

To install Netdata I ssh to the router and then when I was at the terminal on the router I followed for the most part the [Netdata documentation](https://learn.netdata.cloud/docs/agent/packaging/installer/methods/offline) for offline mode. But some of the command I had to modify or adjust. I also had to go to the [Netdata api ](https://api.github.com/repos/netdata/netdata/releases/latest)and do a wget for the url I needed for my router.