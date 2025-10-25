[PROJECT HOME](../index.md)

# Phase 1 - Lab Foundation

## Objective:
Establish the initial network infrastructure of the home lab.

## Overview:
I wanted my homelab to be isolated from the rest of my home network. To accomplish this I needed to establish an additional router/firewall device in my home network, behind which my home lab would reside. This router would run pfSense, which serves as a router and firewall. I also wanted a managed switch that provided high-speed networking along with PoE capability.

---
## Details:
### The Router
After some research, I chose the [Protectli V1211](https://protectli.com/product/v1211/). I've read there could be issues with nesting a second router inside a private network. This is what's referred to a "double NAT". Luckily, I did not run into any issues that required work-arounds such as port forwarding.

### The Switch
For the switch, I went with the [TrendNet TPE-3102WS](https://www.trendnet.com/products/2.5g-managed-poeplus-switch/10-port-multi-gig-web-smart-poeplus-switch-TPE-3102WS). This managed switch allows me to establish VLANs for segmentation, power devices such as access points, and provide both 2.5 and 10 GbE ports for fast internal networking.

### Installation & Setup
Since I ordered a barebones V1211, I needed to add the NVME boot drive. I installed a Crucial P3 Plus 500 GB M.2 drive. After updating the UEFI, I proceeded with pfSense install using a USB drive.

Setting up the managed switch was fairly straightforward. 

---
## Lessons Learned:
asdf
