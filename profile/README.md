# whatsmycli

**Fast, minimal, and extensible cross-platform system information CLI**

One command. All your system info. Any platform.

```bash
whatsmy gpu      # Show GPU information
whatsmy cpu      # Show CPU information
whatsmy ram      # Show memory information
whatsmy weather  # Show weather (via plugin)
```

---

## Why whatsmycli?

Tired of remembering different commands for different system information? `lspci` for GPU, `lscpu` for CPU, different tools on Windows and macOS? **whatsmycli** provides a unified interface:

- **One command pattern** across all platforms (Linux, Windows, macOS)
- **Lightning fast** C++ implementation
- **Highly extensible** through a simple plugin system
- **Open source** - all plugins must be GPLv3-compatible
- **Easy to contribute** - well-documented, clean codebase

## FAQ
**Q: How is this different from neofetch/screenfetch?**  
A: Those are primarily for displaying system info visually. `whatsmy` is designed for quick queries and extensibility through plugins.

**Q: Can I use this in scripts?**  
A: Yes! `whatsmy` is designed to be script-friendly with clean output and proper exit codes.

**Q: How do I request a new built-in command?**  
A: Open an issue on GitHub describing what information you'd like to query. Alternatively, create it as a plugin first!

**Q: Are plugins safe?**  
A: All plugins in the official repository are open-source and verified by maintainers.

## Quick Start

### Installation

**Linux/macOS**:
```bash
curl -sSL https://whatsmycli.github.io/install.sh | sh
```

**Windows** (PowerShell):
```powershell
irm https://whatsmycli.github.io/install.ps1 | iex
```

## Organization Structure

The **whatsmycli** organization consists of three repositories:

### [whatsmy](https://github.com/whatsmycli/whatsmy)
The main application - a cross-platform CLI tool for querying system information.

**Contains**:
- Core application code (C++)
- Plugin loading mechanism
- CMake build system
- GitHub Actions for automated builds

**For**: Users who want the tool, contributors to core functionality

### [plugins](https://github.com/whatsmycli/plugins)
Community-curated repository of verified plugin binaries.

**Contains**:
- Compiled plugin binaries for Linux, Windows, and macOS
- Links to plugin source repositories
- Plugin submission and verification process

**For**: Users who want to extend functionality, plugin authors submitting their work

### [plugin-template](https://github.com/whatsmycli/plugin-template)
Official template for creating GPLv3-compatible plugins.

**Contains**:
- Starter template code
- Example plugin implementation
- Build configuration
- Plugin development documentation

**For**: Developers who want to create their own plugins

## Plugin System

See [plugin-template README](https://github.com/whatsmycli/plugin-template) for detailed instructions.

## Contributing

We welcome contributions! Whether you're:
- Fixing bugs in the core application
- Adding new built-in commands
- Creating new plugins
- Improving documentation
- Reporting issues

Please see:
- [whatsmy/CONTRIBUTING.md](https://github.com/whatsmycli/whatsmy/blob/main/CONTRIBUTING.md) for core contributions
- [plugin-template README](https://github.com/whatsmycli/plugin-template) for plugin development
- [plugins README](https://github.com/whatsmycli/plugins) for plugin submissions

## License

All projects under the **whatsmycli** organization are licensed under the **GNU General Public License v3.0**.

This ensures:
- All code remains open source
- Derivatives must also be open source
- Commercial use is allowed
- Community can freely use, modify, and distribute

See [LICENSE](LICENSE) for full details.

## Credits

Created with the goal of making system information accessible and consistent across all platforms. Built by the community, for the community.

---

**Get started**: Check out [whatsmy](https://github.com/whatsmycli/whatsmy) to install and use the tool, or [plugin-template](https://github.com/whatsmycli/plugin-template) to create your first plugin!

