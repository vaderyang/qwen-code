# Qwen Modified CLI with PCAP Support

This is a modified version of the Qwen CLI that includes enhanced support for handling PCAP (packet capture) files using the `tshark` command-line tool.

## What's Modified

The system prompt has been enhanced to include instructions for handling PCAP files:
- When encountering PCAP files, the AI will use `tshark` for parsing and analysis
- Tshark provides powerful filtering and analysis capabilities for network packet inspection
- Supports protocol analysis and traffic statistics generation

## Usage

To use the modified version instead of the system-wide qwen installation:

```bash
# From the CLI package directory
./qwen_modified [options] [command]

# Examples:
./qwen_modified --version
./qwen_modified --help
./qwen_modified -p "Analyze this pcap file for suspicious traffic patterns"
```

## Version

This modified version is based on qwen-code v0.0.10 with PCAP/tshark enhancements.

## Building

The modified version has already been built. If you need to rebuild after making changes:

```bash
npm run build
```

The `qwen_modified` executable will automatically use the latest built version from the `dist/` directory.