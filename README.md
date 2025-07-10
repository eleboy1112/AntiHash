# AntiHash

<p align="center">
  <img src="https://i.imgur.com/YWLdC8y.png" alt="AntiHash Logo" width="200"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Minecraft-1.20.4-brightgreen?style=for-the-badge&logo=minecraft" alt="Minecraft Version">
  <img src="https://img.shields.io/badge/Server-Paper-blue?style=for-the-badge" alt="Server Type">
  <img src="https://img.shields.io/badge/Version-1.0-orange?style=for-the-badge" alt="Version">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
</p>

## 🛡️ Ultimate Protection Against OpenBukloit Backdoors

**AntiHash** is a cutting-edge Minecraft Paper plugin engineered to detect, prevent, and neutralize backdoors injected by the OpenBukloit tool. Safeguard your server from malicious exploits that can compromise your entire infrastructure.

---

## 🚨 Understanding the OpenBukloit Threat

OpenBukloit is a sophisticated injection tool that compromises legitimate plugins with hidden backdoors. When these infected plugins run on your server:

- **🔓 Privilege Escalation**: Attackers gain operator privileges instantly
- **💬 Chat Command Execution**: Console commands executed through normal chat
- **🕵️ Stealth Operations**: Hidden commands bypass all logging systems  
- **📊 Data Exfiltration**: Server data and configurations can be stolen
- **🎯 Complete Takeover**: Full server control without detection

## ⚡ Key Features

### 🔍 **Advanced Detection Engine**
- Real-time bytecode analysis of plugin JAR files
- Pattern recognition for known OpenBukloit signatures
- Weighted scoring system for accurate threat assessment
- Deep scanning with minimal false positives

### 🛡️ **Active Protection System**
- Blocks backdoor activation attempts in real-time
- Intercepts suspicious chat commands before execution
- Prevents unauthorized privilege escalation
- Maintains server integrity 24/7

### 🎯 **Smart Management**
- Whitelist system for trusted plugins
- Instant admin notifications for security events
- Automatic scanning on server startup
- Configurable sensitivity levels

### 📋 **Comprehensive Logging**
- Detailed threat reports with timestamps
- Plugin integrity verification logs
- Attack attempt documentation
- Audit trail for security compliance

---

## 📥 Installation Guide

### Prerequisites
- Minecraft Paper Server 1.20.4
- Java 17 or higher
- Administrator access to server files

### Installation Steps

1. **Download the Plugin**
   ```
   Download AntiHash.jar from the releases page
   ```

2. **Install on Server**
   ```
   Place AntiHash.jar in your /plugins folder
   ```

3. **Restart Server**
   ```
   Restart your server to activate protection
   ```

4. **Verify Installation**
   ```
   Check console for "AntiHash successfully loaded" message
   ```

---

## 🔧 Command Reference

| Command | Permission | Description |
|---------|------------|-------------|
| `/antihash scan` | `antihash.admin` | Execute full plugin scan |
| `/antihash list` | `antihash.admin` | Display detected threats |
| `/antihash whitelist <add/remove/list> [plugin]` | `antihash.admin` | Manage trusted plugins |
| `/antihash reload` | `antihash.admin` | Reload configuration |
| `/antihash status` | `antihash.admin` | View protection status |
| `/antihash help` | `antihash.admin` | Show command help |

---

## ⚙️ Configuration

```yaml
# ===========================================
# AntiHash Configuration File
# ===========================================

# Scanning Settings
scanning:
  scan-on-startup: true
  deep-scan-enabled: true
  scan-interval-minutes: 30
  minimum-pattern-matches: 3

# Protection Settings  
protection:
  block-suspicious-commands: true
  prevent-privilege-escalation: true
  quarantine-threats: true
  notify-admins: true

# Detection Patterns
detection:
  openbukloit-signatures:
    - "backdoor"
    - "opme"
    - "bukl"
    - "console"
    - "exploit"
    - "admin"
    - "hack"
    - "bypass"
  
  suspicious-methods:
    - "executeCommand"
    - "setOp"
    - "dispatchCommand"
    - "performCommand"

# Whitelist (Trusted Plugins)
whitelist:
  - "AntiHash.jar"
  - "EssentialsX.jar"
  - "Vault.jar"
  - "WorldEdit.jar"
  - "WorldGuard.jar"

# Notification Settings
notifications:
  discord-webhook: ""
  email-alerts: false
  console-logging: true
  admin-broadcast: true
```

---

## 🔒 How AntiHash Works

### 1. **Signature Analysis**
AntiHash uses advanced pattern matching to identify OpenBukloit injection signatures within plugin bytecode.

### 2. **Runtime Protection**
Monitors chat messages and command execution in real-time, blocking suspicious activities before they can execute.

### 3. **Integrity Verification**
Computes cryptographic hashes of plugins to detect unauthorized modifications and tampering.

### 4. **Behavioral Analysis**
Analyzes plugin behavior patterns to identify stealth backdoors that evade signature detection.

### 5. **Threat Quarantine**
Automatically isolates suspicious plugins and prevents them from loading or executing malicious code.

---

## 📊 Performance Impact

| Metric | Impact |
|--------|--------|
| CPU Usage | < 1% during normal operation |
| Memory Usage | ~5MB RAM |
| Startup Time | +2-3 seconds for initial scan |
| Network Impact | Zero |

---

## 🛠️ Troubleshooting

### Common Issues

**False Positives**
- Add legitimate plugins to whitelist
- Adjust `minimum-pattern-matches` in config
- Review detection patterns for conflicts

**Performance Concerns**
- Disable deep scanning if not needed
- Increase scan interval for large servers
- Exclude known safe plugins from scanning

**Integration Problems**
- Ensure Paper server version compatibility
- Check plugin load order in server logs
- Verify permissions are properly configured

---


## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### Ways to Contribute
- 🐛 Report bugs and security vulnerabilities
- 💡 Suggest new features and improvements
- 📝 Improve documentation and guides
- 🧪 Test with different server configurations
- 🔍 Help identify new backdoor patterns


===

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🌟 Support the Project

If AntiHash has helped secure your server, consider:
- ⭐ Starring this repository
- 🐦 Sharing with the Minecraft community
- 💰 [Supporting development](https://github.com/sponsors/yourusername)

---

## 📞 Support & Community

- 📧 **Email**: antihashplugin@gmail.com
- 💬 **Discord**: [Join our community](https://discord.gg/mugcNHKDqB)
- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/eleboy1112/AntiHash/issues)

---

<p align="center">
  <strong>🛡️ Protect your server. Secure your community. Trust AntiHash. 🛡️</strong>
</p>

<p align="center">
  Made with ❤️ for the Minecraft community
</p>
