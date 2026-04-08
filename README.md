# MCP — Custom MCP Servers

A collection of custom-built [Model Context Protocol (MCP)](https://modelcontextprotocol.io) servers built by [Grayson Morris](https://github.com/GraysonMor31).

## What is MCP?

The Model Context Protocol (MCP) is an open standard that lets AI assistants like Claude connect to external tools, data sources, and services. MCP servers expose capabilities (tools, resources, prompts) that AI clients can discover and invoke at runtime.

## Repository Structure

```
MCP/
└── README.md          # This file
```

> Servers will be added here as they are developed.

## Getting Started

Each server lives in its own directory with its own `README.md`, setup instructions, and dependencies. Navigate into a server's directory and follow the instructions there.

### General Prerequisites

- [Node.js](https://nodejs.org) 18+ **or** [Python](https://python.org) 3.11+ depending on the server
- An MCP-compatible client (e.g. [Claude for Desktop](https://claude.ai/download), Claude Code CLI)

## Usage with Claude

To connect a server to Claude for Desktop, add an entry to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "your-server-name": {
      "command": "node",
      "args": ["/path/to/server/index.js"]
    }
  }
}
```

Refer to each server's individual README for the exact command and configuration options.

## Author

**Grayson Morris**
- GitHub: [@GraysonMor31](https://github.com/GraysonMor31)
- Site: [graysonmor31.github.io](https://graysonmor31.github.io)
- Company: Sierra Nevada Corporation

## License

MIT
