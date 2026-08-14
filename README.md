# Tor Bridges Collector v2

This repository automatically collects, validates, and archives Tor bridges. A GitHub Action runs every 5 minutes to fetch new bridges from the official Tor Project.

## Important Notes on IPv6 & WebTunnel

1.  **IPv6 Instability:** IPv6 bridges are significantly fewer in number and are often more susceptible to blocking or connection instability compared to IPv4.
2.  **WebTunnel Overlap:** WebTunnel bridges often use the same endpoint domain for both IPv4 and IPv6. Consequently, the IPv6 list is frequently identical to or a subset of the IPv4 list.
3.  **Recommendation:** For the most reliable connection, **prioritize using IPv4 bridges**. Use IPv6 only if IPv4 is completely inaccessible on your network.

## Bridge Lists

### Tested & Active (Recommended)
These bridges from the archive have passed a TCP connectivity test (3 retries, 10s timeout) during the last run.

| Transport | IPv4 (Tested) | Count | 
| :--- | :--- | :--- |
| **obfs4** | [obfs4_tested.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/obfs4_tested.txt) | **206** |
| **WebTunnel** | [webtunnel_tested.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/webtunnel_tested.txt) | **107** |
| **Vanilla** | [vanilla_tested.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/vanilla_tested.txt) | **58** |

### Fresh Bridges (Last 72 Hours)
Bridges discovered within the last 3 days.

| Transport | IPv4 (72h) | Count | IPv6 (72h) | Count |
| :--- | :--- | :--- | :--- | :--- |
| **obfs4** | [obfs4_72h.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/obfs4_72h.txt) | **2** | [obfs4_ipv6_72h.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/obfs4_ipv6_72h.txt) | **2** |
| **WebTunnel** | [webtunnel_72h.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/webtunnel_72h.txt) | **2** | [webtunnel_ipv6_72h.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/webtunnel_ipv6_72h.txt) | **2** |
| **Vanilla** | [vanilla_72h.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/vanilla_72h.txt) | **2** | [vanilla_ipv6_72h.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/vanilla_ipv6_72h.txt) | **1** |

### Full Archive (Since 2026-01-30)
History of all collected bridges.

| Transport | IPv4 | Count | IPv6 | Count |
| :--- | :--- | :--- | :--- | :--- |
| **obfs4** | [obfs4.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/obfs4.txt) | **342** | [obfs4_ipv6.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/obfs4_ipv6.txt) | **174** |
| **WebTunnel** | [webtunnel.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/webtunnel.txt) | **134** | [webtunnel_ipv6.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/webtunnel_ipv6.txt) | **134** |
| **Vanilla** | [vanilla.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/vanilla.txt) | **115** | [vanilla_ipv6.txt](https://raw.githubusercontent.com/scriptzteam/Tor-Bridges-Collector-v2/refs/heads/main/bridges/vanilla_ipv6.txt) | **35** |

## 🔥 Keep This Project Going!

If you're finding this useful, please show your support:

⭐ **Star the repository on GitHub**

Your stars fuel our motivation to keep improving!

## Disclaimer
This project is for educational and archival purposes. Please use these bridges responsibly.
