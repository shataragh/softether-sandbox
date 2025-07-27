# 🛡️ SoftEther VPN Lab in GitHub Codespaces

[![Codespaces Ready](https://img.shields.io/badge/GitHub-Codespaces-blue?logo=github)](https://github.com/features/codespaces)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
[![Security Status](https://img.shields.io/badge/Security-Proactive-red?logo=security)](SECURITY.md)

Deploy a full-featured SoftEther VPN server inside GitHub Codespaces — complete with CLI management, source build, and optional stealth tunneling.

🔐 Tailored for developers in censorship-prone regions or privacy-first sandbox setups.

---

## 📸 Preview

![SoftEther Codespace Demo](https://uploadkon.ir/uploads/524b08_25VPN.png)  
> _SoftEther VPN server with stealth extensions running inside GitHub Codespaces_

---

## 🚀 Table of Contents

- [✅ Features](#features)
- [🧰 Quick Start](#quick-start)
- [📕 Usage Guide](USAGE.md)
- [⚙️ Advanced Configuration](ADVANCED-CONFIG.md)
- [🛡️ Security Notes](SECURITY.md)
- [⚠️ Known Limitations](LIMITATIONS.md)
- [📄 License](LICENSE.md)
- [👤 Credits & Contact](CONTACT.md)

---

## 📦 Features

| Feature | Description |
|--------|-------------|
| 🧑‍💻 CLI VPN Management | Configure hubs and users via `vpncmd` |
| 🕵️ Stealth Tunneling | Enable `obfs4`, `stunnel`, WebSocket over TLS |
| 🔐 Secure Admin Entry | Password-protected `localhost:5555` |
| 💡 GitHub Codespaces-Ready | No external scripts or GUI dependencies |
| 🔄 Reproducible Builds | CMake + submodules for consistent setup |

---

## 🧰 Quick Start

Get up and running inside GitHub Codespaces or locally:

```bash
# Clone repo and enter
git clone https://github.com/shataragh/softether-sandbox.git
cd softether-sandbox/SoftEtherVPN

# Init and compile
git submodule update --init --recursive
./configure
make -C build

# Launch VPN server and CLI
cd build
./vpnserver start
./vpncmd
