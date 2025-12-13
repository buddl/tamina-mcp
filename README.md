# Tamina MCP Server

This repository provides information about the MCP (Model Context Protocol) server for [Tamina](https://tamina.app), a website for booking appointments and making reservations.

## Overview

Tamina is a comprehensive platform for managing appointments and reservations. The MCP server allows AI assistants like ChatGPT, Claude, and Copilot to interact with Tamina's services programmatically.

## Server Details

- **MCP Server URL**: `https://tamina.app/api/mcp`
- **Authentication**: OAuth with dynamic client registration
- **Status**: Public

## Features

The Tamina MCP server supports:
- OAuth authentication for secure access
- Dynamic client registration
- Integration with popular AI assistants and custom connectors

## How to Connect

### Connecting to ChatGPT, Claude, or Copilot

When you connect this MCP server as a custom connector to ChatGPT, Claude, Copilot, or other AI assistants:

1. Add the MCP server URL: `https://tamina.app/api/mcp`
2. You will be prompted to sign in to [tamina.app](https://tamina.app)
3. Complete the OAuth authentication flow
4. Once authenticated, the AI assistant can interact with your Tamina account

### Authentication

The server uses OAuth with dynamic client registration, which means:
- You need to authenticate via the Tamina website on first connection
- Your credentials are managed securely through OAuth
- The server will automatically register your client application

## Support

For more information about Tamina and its services, visit [https://tamina.app](https://tamina.app).

## License

MIT License - see [LICENSE](LICENSE) for details.
