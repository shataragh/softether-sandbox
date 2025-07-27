# ⚙️ Advanced Configuration Options

Deepen your privacy posture with resilient obfuscation and tunneling techniques designed to bypass deep packet inspection (DPI), evade surveillance, and improve operational safety in censorship-prone environments.

---

## 🧰 Stealth Wrapper Overview

Use the `stealth-wrapper.sh` script to launch different obfuscation modes. Each method alters traffic fingerprints to help VPNs blend in or resist protocol detection.

### 🕵️‍♂️ Available Modes

```bash
# 🦎 Launch obfs4proxy to disguise VPN traffic
bash tools/stealth-wrapper.sh --obfs4

# 🔐 Add SSL/TLS layer using stunnel
bash tools/stealth-wrapper.sh --stunnel

# 🌐 Connect VPN via browser-mimicking WebSocket wrapped in TLS
bash tools/stealth-wrapper.sh --wss
```

## 📗 Usage Instructions
To view chaining options, proxy layering, and advanced help:

```bash
bash tools/stealth-wrapper.sh --help
```
