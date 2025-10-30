![Banner](https://raw.githubusercontent.com/whatsmycli/whatsmycli/main/.github/profile/banner.png)

> Fast, minimal, and extensible cross-platform system information CLI

One command pattern across Linux, Windows, and macOS. Everything is a plugin.

```bash
whatsmy gpu      # Show GPU information
whatsmy cpu      # Show CPU information  
whatsmy weather  # Show weather
```

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

## Organization

The **whatsmycli** organization consists of three repositories:

### [whatsmy](https://github.com/whatsmycli/whatsmy)
Main CLI application. Loads and executes plugins.

### [plugins](https://github.com/whatsmycli/plugins)
Community plugin repository. Verified binaries for Linux, Windows, and macOS.

### [plugin-template](https://github.com/whatsmycli/plugin-template)
Template for creating your own plugins.

## License

GNU General Public License v3.0 - All code is open source.
