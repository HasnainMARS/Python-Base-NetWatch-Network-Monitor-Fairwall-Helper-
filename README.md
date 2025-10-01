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

---

## 🤝 Contributing

Contributions are welcome! Fork the repo, create a branch, open a PR. See `CONTRIBUTING.md` for details.

---

## 🧾 License

MIT — see `LICENSE`.


### Final notes

* Replace `https://github.com/<your-username>/netwatch.git` in the README with your real GitHub URL.
* The Flask UI is intentionally minimal and **must not** be exposed without adding authentication and HTTPS.
* Want me to also add the `netwatch_fairwall.py` full script into this paste? I can add it into the repo file content next.

---

Happy to keep going — I can now:

* Add the full `netwatch_fairwall.py` script into the repo (ready to paste),
* Create a ready-to-copy `LICENSE` (MIT),
* Generate a `.github/workflows/ci.yml` basic CI that runs lint/tests.

Tell me which of those you want next and I will add them here.

---

## ADDITIONAL FILES (LICENSE, CI, netwatch_fairwall.py, requirements.txt)

### LICENSE (MIT)

```text
MIT License

Copyright (c) 2025 HasnainMARS

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

    parser.add_argument("--periodic-arp", action="store_true", help="Run
```
