# ThreadBridge MCP Server for Zed

A [Zed](https://zed.dev) extension that provides persistent AI memory through the [Model Context Protocol](https://modelcontextprotocol.io/).

ThreadBridge remembers context across conversations using hybrid semantic search (Arctic Embed + BM25 + RRF) with a cognitive decay model (BLL).

## Installation

1. Open Zed
2. Go to **Extensions** (cmd+shift+x)
3. Search for "ThreadBridge"
4. Click **Install**

The extension will automatically download the appropriate binary for your platform.

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
