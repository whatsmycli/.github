![Banner](https://raw.githubusercontent.com/whatsmycli/.github/refs/heads/main/profile/banner.png)

One command pattern across Linux, Windows, and macOS. Everything is a plugin.

```bash
whatsmy gpu      # Show GPU information
whatsmy cpu      # Show CPU information  
whatsmy weather  # Show weather
whatsmy help     # Show help
whatsmy version  # Show version
```

## Why whatsmycli?

Tired of remembering different commands for different system information? `lspci` for GPU, `lscpu` for CPU, different tools on Windows and macOS? **whatsmycli** provides a unified interface.

**Installation:**

Linux/macOS:
```bash
curl -sSL https://raw.githubusercontent.com/whatsmycli/whatsmy/main/install.sh | bash
```

Windows (PowerShell):
```powershell
irm https://raw.githubusercontent.com/whatsmycli/whatsmy/main/install.ps1 | iex
```

## Organization

The **whatsmycli** organization consists of four repositories:

### [whatsmy](https://github.com/whatsmycli/whatsmy)
Main CLI application. Loads and executes plugins.

### [plugins](https://github.com/whatsmycli/plugins)
Community plugin repository. Verified binaries for Linux, Windows, and macOS.

### [plugin-template](https://github.com/whatsmycli/plugin-template)
Template for creating your own plugins. Write your first plugin in under 10 minutes.

### [docs](https://github.com/whatsmycli/docs)
Complete documentation including plugin API reference and architecture guides.
