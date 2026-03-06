# ThreadBridge MCP Server for Zed

A [Zed](https://zed.dev) extension that provides persistent AI memory through the [Model Context Protocol](https://modelcontextprotocol.io/).

ThreadBridge remembers context across conversations using hybrid semantic search (Arctic Embed + BM25 + RRF) with a cognitive decay model (BLL).

## Installation

### From Extension Marketplace

1. Open Zed
2. Go to **Extensions** (cmd+shift+x)
3. Search for "ThreadBridge"
4. Click **Install**

ThreadBridge is now available in the Zed Extension Marketplace. The extension will automatically download the appropriate binary for your platform.

### Local Installation (Dev)

Dev extensions are compiled locally by Zed, so this installation method requires Rust via [rustup](https://www.rust-lang.org/tools/install). Rust is not required when installing ThreadBridge from the Zed Extension Marketplace.

1. Clone this repository:
   ```sh
   git clone https://github.com/dereklei12/zed-mcp-server-threadbridge.git
   ```

2. In Zed, open the command palette (cmd+shift+p) and run **zed: install dev extension**, then select the cloned directory.

3. The extension will automatically download the `mcp-threadbridge` binary from [GitHub Releases](https://github.com/dereklei12/mcp-threadbridge/releases) on first use.

## Supported Platforms

- macOS (Apple Silicon)
- Linux (x86_64)
- Windows (x86_64)

## MCP Tools

| Tool | Description |
|------|-------------|
| `load_thread` | Load saved conversation context for a project |
| `save_thread` | Save current conversation context |
| `search_memory` | Semantic search across project memory |

## Configuration

Optionally set a `project_path` in Zed settings to specify which project's memory to use. If not set, the current working directory is used.

## License

MIT
