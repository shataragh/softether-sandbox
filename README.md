# 🛡️ SoftEther VPN Lab in GitHub Codespaces

This project sets up a fully functional SoftEther VPN server inside GitHub Codespaces — complete with build-from-source, user creation, and optional stealth tunneling.

## 📦 Features

- Build SoftEther from official source using CMake
- Run server entirely in-browser (Codespaces)
- Launch `vpncmd` to manage hubs, users, SecureNAT
- Optional extensions: `stunnel`, `obfs4proxy`, WebSocket tunneling

## 🧰 Quick Start

```bash
# Clone it
git clone https://github.com/shataragh/softether-sandbox.git
cd softether-sandbox/SoftEtherVPN

# Initialize submodules & build
git submodule update --init --recursive
./configure
make -C build

# Run the server
cd build
./vpnserver start
./vpncmd
