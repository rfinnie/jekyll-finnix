---
date: 2008-06-02 09:05:13
layout: post
title: Finnix and Debian's OpenSSL Vulnerability
wp_id: 68
---
All versions of Finnix from 89.0 to 91.1 (inclusive) contain the [Debian OpenSSL predictable RNG vulnerability](https://lists.debian.org/debian-security-announce/2008/msg00152.html). The fix will be included with the next scheduled (approximately quarterly) release of Finnix in the next few weeks. In the meantime, if you use any OpenSSL-related programs (openssl itself, ssh, openvpn, etc) on Finnix, be sure to do the following as soon as you boot Finnix:

`apt-get update && apt-get install libssl0.9.8`

Finnix does not include any pre-generated keys, but any keys generated on Finnix with a vulnerable OpenSSL will be vulnerable.
