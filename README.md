# 🛡️ SoftEther VPN Lab in GitHub Codespaces

[![Codespaces Ready](https://img.shields.io/badge/GitHub-Codespaces-blue?logo=github)](https://github.com/features/codespaces)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Security Status](https://img.shields.io/badge/Security-Proactive-red?logo=security)](https://www.linkedin.com/in/sir1/)

Run a full-featured SoftEther VPN server inside GitHub Codespaces — complete with source build, CLI management, and optional stealth tunneling.  
This lab is tailored for developers working under censorship, privacy risk, or sandbox experimentation.

---

## 📸 Preview

![SoftEther Codespace Demo](https://uploadkon.ir/uploads/524b08_25VPN.png)  
> _SoftEther VPN server with stealth-ready features running fully inside Codespaces_

---

## 🚀 Table of Contents

- [Features](#-features)
- [Quick Start](#-quick-start)
- [Usage Guide](#-usage-guide)
- [Advanced Configuration](#-advanced-configuration)
- [Security Notes](#-security-notes)
- [Known Limitations](#-known-limitations)
- [License](#-license)
- [Credits & Contact](#-credits--contact)

---

## 📦 Features

| Feature | Description |
|--------|-------------|
| ✅ VPN over Codespaces | SoftEther built from source, hosted inside GitHub IDE |
| 🧑‍💻 CLI management (`vpncmd`) | Create hubs, users, enable SecureNAT |
| 🕵️‍♂️ Stealth-ready tunnels | Optional: `stunnel`, `obfs4proxy`, WebSocket over TLS |
| 🔐 Admin-restricted access | Password-protected `localhost:5555` connection |
| 📄 Inline Documentation | Everything inside one Markdown file for clarity |
| 🔄 Reproducible Workflow | No external configs or setup scripts required |

---

## 🧰 Quick Start

```bash
# Clone & enter repo
git clone https://github.com/shataragh/softether-sandbox.git
cd softether-sandbox/SoftEtherVPN

# Initialize and build
git submodule update --init --recursive
./configure
make -C build

# Launch SoftEther Server & CLI
cd build
./vpnserver start
./vpncmd
