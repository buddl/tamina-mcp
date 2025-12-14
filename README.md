# Tamina MCP Server

This repository provides the MCP (Model Context Protocol) server configuration for Tamina, a powerful platform available at [https://tamina.app](https://tamina.app). The MCP server enables AI assistants like ChatGPT, Claude, and GitHub Copilot to connect to Tamina's services and leverage its capabilities within your AI-powered workflows.

## About Tamina

Tamina is a web app to make reservations and book appointments at local businesses. Reserve a table in a restaurant, reserve a room in a hotel, order a taxi, book an appointment at a hair salon, a nail studio, a doctor and many more.
The Tamina MCP server acts as a bridge between AI platforms and Tamina's services. By connecting to this MCP server, AI assistants can search for local businesses and make reservations directly during your conversations without visiting the website. The MCP server is hosted at **https://tamina.app/api/mcp** and requires authentication before use.

## Prerequisites

Before connecting to the Tamina MCP server, you need:

- An active account on [Tamina](https://tamina.app)
- Valid authentication credentials from your Tamina account
- An AI platform that supports MCP (Model Context Protocol)

## Connecting to ChatGPT

ChatGPT currently supports MCP servers through custom implementations and API integrations. To connect the Tamina MCP server to ChatGPT, you will need to use the OpenAI API with a custom client that supports the Model Context Protocol. This typically involves:

1. Setting up a custom application that communicates with both ChatGPT's API and the Tamina MCP server.
2. Configuring your application to use the MCP server URL: `https://tamina.app/api/mcp`
3. Implementing authentication with your Tamina credentials in your application.
4. Routing relevant context and requests through the MCP protocol.

For direct integration, you may need to wait for official MCP support in ChatGPT or use third-party tools that bridge ChatGPT with MCP servers.

## Connecting to Claude

Claude Desktop supports MCP servers through configuration files. To connect the Tamina MCP server to Claude Desktop:

1. Locate your Claude Desktop configuration file:
   - On macOS: `~/Library/Application Support/Claude/claude_desktop_config.json`
   - On Windows: `%APPDATA%\Claude\claude_desktop_config.json`
   - On Linux: `~/.config/Claude/claude_desktop_config.json`

2. Open the configuration file in a text editor.

3. Add the Tamina MCP server to the `mcpServers` section:

```json
{
  "mcpServers": {
    "tamina": {
      "url": "https://tamina.app/api/mcp",
      "authentication": {
        "type": "bearer",
        "token": "YOUR_TAMINA_AUTH_TOKEN"
      }
    }
  }
}
```

4. Replace `YOUR_TAMINA_AUTH_TOKEN` with your actual Tamina authentication token.

5. Save the configuration file and restart Claude Desktop.

6. Claude will now have access to Tamina's services through the MCP connection.

## Connecting to GitHub Copilot

GitHub Copilot integration with MCP servers is an emerging area. Currently, GitHub Copilot does not have native built-in support for connecting to external MCP servers through Visual Studio Code settings. However, you can leverage MCP functionality in your development workflow through these approaches:

1. **Use MCP-compatible extensions**: Look for Visual Studio Code extensions that support the Model Context Protocol and can integrate with GitHub Copilot's functionality.

2. **Custom integration**: Develop a custom VS Code extension that:
   - Connects to the Tamina MCP server at `https://tamina.app/api/mcp`
   - Authenticates using your Tamina credentials
   - Provides context to GitHub Copilot through the VS Code extension API

3. **API-based approach**: Create a local service that bridges GitHub Copilot's capabilities with the Tamina MCP server, allowing you to access Tamina's functionality alongside Copilot's code suggestions.

As MCP adoption grows, more direct integration options may become available. Check the GitHub Copilot documentation and Tamina's official channels for updates on native MCP support.

## Authentication

The Tamina MCP server requires authentication upfront before any requests can be made. You will need to provide valid credentials from your Tamina account during the connection setup process. The authentication ensures secure access to Tamina's services and maintains the integrity of your data.

To obtain your authentication credentials:

1. Log in to your account at [https://tamina.app](https://tamina.app)
2. Navigate to your account settings or API credentials section
3. Generate or retrieve your MCP authentication token
4. Use these credentials when configuring the MCP connection in your AI platform

## Server URL

The official Tamina MCP server URL is:

```
https://tamina.app/api/mcp
```

Always use this exact URL when configuring MCP connections to ensure proper communication with Tamina's services.

## Support

For issues, questions, or additional support regarding the Tamina MCP server:

- Visit the [Tamina website](https://tamina.app)
- Check the Tamina documentation for detailed API information
- Contact Tamina support through their official channels

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
