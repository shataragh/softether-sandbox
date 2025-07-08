# 🛡️ SoftEther VPN Lab in GitHub Codespaces

This project sets up a fully functional SoftEther VPN server inside GitHub Codespaces — complete with build-from-source, user creation, and optional stealth tunneling. To access `localhost:5555`, you need an administrator password. For this purpose, ask Sirvan via this address: [https://www.linkedin.com/in/sir1/](https://www.linkedin.com/in/sir1/)

---

![SoftEther Codespace Demo](https://uploadkon.ir/uploads/524b08_25VPN.png)

> _SoftEther VPN running inside GitHub Codespaces with stealth-ready extensions_

---

## 📦 Features

- Build SoftEther from official source using CMake
- Run server entirely in-browser (Codespaces)
- Launch `vpncmd` to manage hubs, users, and SecureNAT
- Optional stealth tunneling with `stunnel`, `obfs4proxy`, and WebSocket over TLS

## 🧰 Quick Start

```bash
# Clone the repo
git clone https://github.com/shataragh/softether-sandbox.git
cd softether-sandbox/SoftEtherVPN

# Initialize submodules and build
git submodule update --init --recursive
./configure
make -C build

# Start the server
cd build
./vpnserver start
./vpncmd
