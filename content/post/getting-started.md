---
title: Getting started
description: Prelude
date: 2025-01-29T21:02:00+01:00
---

# SSH key
To connect to the server, send me the OpenSSH public key ([not PuTTY](//gist.github.com/stefhen/5b3cf11b52eb7764fee7a7d30430bb2a)).

# Domain
I'm also delegating the third level domain to you.
Send me the desired name (e.g. puppy.RADU.GA) and NS records.
You can find NS records from your DNS hoster - I highly recommend [Hurricane Electric](//dns.he.net) (you might be thinking of Cloudflare, but they don't allow you to host subdomains).

# Records
Instead of adding A and AAAA records, I suggest adding CNAME records to the existing ones.
- \<name\>.ip.radu.ga (IPv4 and IPv6 records)
- \<name\>.ipv4.radu.ga (IPv4 record)
- \<name\>.ipv6.radu.ga (IPv6 record)
- \<name\>.cdn.radu.ga (IPv6 record, proxified*)

# IP
Along with the VPS, I also provide one IPv6 address (e.g. 2607:5300:60:6a3d::100) and 100 IPv4 ports (e.g. 10000-10099).
The IPv4 address is one for everyone and is tied to the hypervisor (which also proxies 100 specific ports to the VPS).
But if you use a proxified DNS record (e.g. \<name\>.cdn.radu.ga), your server will be available on any ports even for IPv4 clients (HTTP/s only).
