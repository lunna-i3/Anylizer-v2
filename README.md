# Anylizer V2 | Discord Raid Bot

<div align="center">

![Anylizer](https://img.shields.io/badge/Anylizer-v2.0-red?style=for-the-badge&logo=discord)
![Python](https://img.shields.io/badge/Python-3.8%2B-green?style=for-the-badge&logo=python)
![CLI](https://img.shields.io/badge/CLI-Raid%20Tool-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**⚡ Advanced CLI Discord Raid Bot with Multi-Bot Support and Server Management**

*Powerful raid tool for educational purposes and authorized testing*

[Features](#-features) • [Installation](#-installation) • [Quick Start](#-quick-start) • [Raid Commands](#-raid-commands) • [Disclaimer](#-legal-disclaimer)

</div>

## ⚡ Overview

**Anylizer V2** is a powerful CLI-based Discord raid bot designed for advanced server testing and educational purposes. Featuring multi-bot support, real-time monitoring, and comprehensive raid capabilities, it provides complete control over Discord servers through an intuitive command-line interface.

> ⚠️ **WARNING**: This tool is for educational and authorized testing purposes only. Misuse may violate Discord's Terms of Service.

## 🎯 Features

### 🤖 Multi-Bot Raid System
- **🔀 Bot Switcher**: Instant switching between multiple raid bots
- **📊 Token Manager**: Secure storage and management of bot tokens
- **🌐 Cross-Server Coordination**: Synchronized operations across multiple servers
- **📈 Real-time Analytics**: Live bot status and server statistics

### 💥 Raid Capabilities
- **☢️ Server Nuking**: Complete server takeover and restructuring
- **📢 Mass Messaging**: Coordinated spam across multiple channels
- **🔧 Channel Management**: Bulk create/delete channels
- **👥 User Management**: Mass nickname changes and user targeting
- **🌐 Webhook Spam**: Persistent messaging through webhooks

### 🔍 Intelligence Gathering
- **🕵️ Server Recon**: Detailed server information and architecture
- **👮 Staff Monitoring**: Real-time admin and moderator tracking
- **🔐 Permission Analysis**: Comprehensive security auditing
- **📊 Channel Mapping**: Complete server structure analysis

### 🎨 Advanced CLI Interface
- **🌈 Colorful Output**: Formatted terminal with ANSI colors
- **⚡ Real-time Chat**: Direct messaging through bot interface
- **🛡️ Recovery System**: Safe fallback for configuration issues
- **🔧 Config Management**: Dynamic settings modification

## 📋 Requirements

- **Python 3.8+**
- **discord.py** library
- **requests** library
- **Discord Bot Token(s)** with privileged intents

## 🔧 Installation

### 1. Clone & Setup
```bash
git clone https://github.com/lunna-i3/anylizer.git
cd anylizer
python3 -m pip install discord.py requests asyncio
```

### 2. Bot Configuration
1. Create applications at [Discord Developer Portal](https://discord.com/developers/applications)
2. Enable **ALL** privileged gateway intents for each bot
3. Generate bot tokens for raid operations

## 🚀 Quick Start

### First Time Setup

1. **Launch the raid tool:**
```bash
python main.py
```

2. **Add your raid bots:**
```bash
switch add raidbot1 YOUR_FIRST_BOT_TOKEN
switch add raidbot2 YOUR_SECOND_BOT_TOKEN
```

3. **Switch to your primary raid bot:**
```bash
switch to raidbot1
```

4. **Begin server reconnaissance:**
```bash
.servers
.check all 1
.check staff 1
```

## 💥 Raid Commands

### 🎯 Server Takeover Commands

| Command | Description | Usage |
|---------|-------------|-------|
| **`.nuke <server>`** | ☢️ Complete server takeover | `.nuke 1` |
| **`.clean <server>`** | 🗑️ Delete all channels | `.clean 1` |
| **`.create <server> <type> <name>`** | 📝 Create channels | `.create 1 text raid-channel` |
| **`.delete <server> <channel_id>`** | ❌ Delete specific channel | `.delete 1 123456789` |

### 🔍 Intelligence Commands

| Command | Description | Usage |
|---------|-------------|-------|
| **`.check staff <server>`** | 👮 Track online staff | `.check staff 1` |
| **`.check perms <server>`** | 🔐 Analyze bot permissions | `.check perms 1` |
| **`.check chans <server>`** | 📊 List all channels | `.check chans 1` |
| **`.check all <server>`** | 🕵️ Full server recon | `.check all 1` |

### 💬 Communication Commands

| Command | Description | Usage |
|---------|-------------|-------|
| **`.talk <channel_id>`** | 💬 Chat through bot | `.talk 123456789` |
| **`.invite <server>`** | 📨 Generate invite link | `.invite 1` |

## ⚙️ Raid Configuration

### Nuke Settings (`config/settings.json`)

```json
{
  "bot_settings": {
    "nuke": {
      "server_name": "ANYLIZER RAIDED",
      "username": "RAIDED BY ANYLIZER",
      "change_usernames": true,
      "change_servername": true,
      "messages": {
        "content": "🚀 SERVER RAIDED BY ANYLIZER V2 🚀\n||@everyone @here||",
        "bot_spam": true,
        "bot_messages_per_channel": 5,
        "webhooks_spam": true,
        "webhook_messages_per_channel": 10
      },
      "channels": {
        "number": 15,
        "name": "raided-by-anylizer"
      }
    }
  }
}
```

### 🔧 Real-time Configuration

Modify raid settings on-the-fly:
```bash
# Change raid message
do set bot_settings.nuke.messages.content "YOUR_RAID_MESSAGE"

# Adjust channel count
do set bot_settings.nuke.channels.number 20

# Toggle features
do set bot_settings.nuke.change_usernames true
```

## 🔄 Bot Management

### Multi-Bot Operations
```bash
# List all raid bots
switch list

# Add new raid bot
switch add bot3 NEW_TOKEN

# Switch between bots
switch to bot2

# Remove compromised bot
switch remove bot1
```

## 🛡️ Safety & Stealth

### Operational Security
- **🔄 Bot Rotation**: Switch between multiple accounts
- **📊 Permission Checking**: Verify bot access before operations
- **⏱️ Rate Limit Management**: Built-in delay between actions
- **🔒 Error Handling**: Silent failure on permission denied

### Recovery Features
- **📁 Auto-backup**: Configuration backups before modifications
- **🔄 Reset Capability**: Restore default settings instantly
- **🚨 Safe Mode**: Recovery shell for configuration issues

## 🎯 Advanced Raid Strategies

### 1. Reconnaissance Phase
```bash
.servers                    # List accessible servers
.check staff 1              # Identify online staff
.check perms 1              # Verify bot permissions
```

### 2. Preparation Phase
```bash
.clean 1                    # Clear existing channels
.invite 1                   # Generate backup invite
```

### 3. Execution Phase
```bash
.nuke 1                     # Execute full takeover
```

### 4. Persistence Phase
```bash
.talk 123456789             # Maintain communication
.create 1 text control      # Create control channels
```

## ❗ Troubleshooting

### Common Raid Issues

1. **Bot Lacks Permissions**
   ```bash
   .check perms 1           # Verify permissions
   # Ensure bot has ADMINISTRATOR privilege
   ```

2. **Rate Limited**
   - Tool includes automatic rate limit handling
   - Use multiple bots for distributed operations

3. **Configuration Errors**
   ```bash
   do reset all             # Reset to defaults
   # Check config/.settings.json.bak for backups
   ```

## ⚠️ Legal Disclaimer

**THIS TOOL IS FOR EDUCATIONAL AND AUTHORIZED TESTING PURPOSES ONLY**

### ✅ Permitted Uses:
- Security research and education
- Authorized penetration testing
- Personal server testing (with explicit permission)
- Bot development learning

### ❌ Prohibited Uses:
- Unauthorized server access
- Malicious attacks on communities
- Harassment or disruptive behavior
- Any illegal activities

**The developers are not responsible for misuse of this tool. Users are solely responsible for complying with Discord's Terms of Service and applicable laws.**

## 🔧 Development

### Contributing
We welcome contributions to improve Anylizer V2:
- Bug reports and fixes
- Feature suggestions
- Code optimization
- Documentation improvements

### Building from Source
```bash
git clone https://github.com/lunna-i3/anylizer.git
cd anylizer
# Review and modify code as needed
python main.py
```

## 📞 Support

### Getting Help
1. **Built-in Help**: Use `help` and `switch manual` commands
2. **Configuration**: Check `config/settings.json` for settings
3. **Recovery**: Access recovery mode for configuration issues

### Community
- **GitHub Issues**: Bug reports and feature requests
- **Documentation**: This README and code comments
- **Educational Resources**: Discord API documentation

---

<div align="center">

**🔥 BUILT FOR EDUCATIONAL PURPOSES - USE RESPONSIBLY 🔥**

**Made with ❤️ by imluxa**

*⚠️ Use only on authorized servers. Respect community guidelines and laws.*
*writen by: deepseek, i've no clue what he wrote here...*
</div>
