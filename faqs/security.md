# Frequently Asked Questions About Security and Reliability

---
status: "ongoing"
date: 2025-06-11
---

We take security very seriously and believe that using FAIR will fortify the WordPress supply chain. Using signing and authentication, FAIR mitigates unapproved takeovers or nulling of plugins or themes, restoring trust in deliverables.

One of the main reasons the FAIR project exists is to ensure that all WordPress users, regardless of their host, continue to have access to WordPress, theme and plugin updates. This will give developers and users confidence in the security of their software.

## Could FAIR increase the risk of a DDoS attack on WordPress.org?

No. The plugin and theme repository mirroring part of FAIR currently uses AspirePress, which caches plugins and themes, significantly reducing traffic to WordPress.org. Their mirror has been running without issue since the middle of January 2025. Other APIs, such as the events listing or BrowseHappy, fully replace the official ones. This effectively reduces load rather than increasing it, as many APIs are no longer sending any traffic to WordPress.org at all.

## If you use AspirePress, how does AspirePress handle load to avoid overwhelming WordPress.org?

AspireSync, used by AspirePress to fetch WordPress.org data, employs strict rate-limiting (no more than 10 simultaneous requests) and pauses to minimize impact. WordPress.org also has its own traffic shaping measures to manage potential overloads.

The FAIR and AspirePress projects will allow anyone who wants to set up their mirror to get their initial data from us rather than from WordPress.org, to protect .org.

## How secure is FAIR compared to centralized hosting on WordPress.org?

FAIR and AspirePress incorporate rigorous security practices and leverage infrastructure like Fastly CDN for improved reliability and security. with the help of industry experts, we are continually adapting our security measures.

We look forward to actively collaborating with the WordPress.org Security Team to enhance overall supply chain security.
