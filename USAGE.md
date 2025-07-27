# 📕 SoftEther VPN Usage Guide

This guide shows you how to use the CLI (`vpncmd`) to manage VPN hubs, users, and network settings in your GitHub Codespace.

## 🔧 Common Tasks

```bash
# Create a new VPN hub
HubCreate myVPNhub /PASSWORD:adminpass

# Enable NAT + DHCP for auto-routing
SecureNatEnable myVPNhub

# Create a user inside the hub
UserCreate alice /GROUP:none /REALNAME:"Alice Demo" /NOTE:"Beginner test"
UserPasswordSet alice /PASSWORD:alicepass
