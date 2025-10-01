# 🚨 NetWatch — Network Monitor & Fairwall Helper 🛡️

> Lightweight, safe, and admin-friendly toolkit to monitor devices on a Wi‑Fi / LAN and apply host-level firewall blocks.

## ✨ Highlights

- 🔍 **Passive Wi‑Fi monitoring** — sniff beacon frames (SSID / BSSID) and client frames (requires interface in monitor mode).
- 🕵️‍♂️ **LAN discovery** — fast ARP scans and ICMP ping scans for local subnets.
- 🧾 **Unified device registry** — MAC → IP → SSID mapping with `last_seen` timestamps.
- 🔒 **Safe fairwall actions** — call OS firewall (iptables on Linux, `netsh` on Windows) to block/unblock IPs.
- 🧰 **Single script, CLI driven** — modular flags so you run only the features you need.
- ♻️ **Non-invasive** — no deauthentication, no ARP spoofing, no packet injection included.

---


## ✅ Best practices & safety

* Only run discovery & blocking on networks you **own or administer**. Unauthorized scanning or interference can be illegal.
* This project intentionally **excludes** deauthentication, ARP spoofing, or other disruptive attacks. If you need client isolation, prefer router/AP-level blocking.
* Always keep a separate admin session (e.g., wired connection or console) while experimenting with firewall rules.


