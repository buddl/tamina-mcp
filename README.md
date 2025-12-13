# Tamina MCP Server

This repository provides the MCP (Model Context Protocol) server configuration for Tamina, a powerful platform available at [https://tamina.app](https://tamina.app). The MCP server enables AI assistants like ChatGPT, Claude, and GitHub Copilot to connect to Tamina's services and leverage its capabilities within your AI-powered workflows.

## About Tamina MCP

The Tamina MCP server acts as a bridge between AI platforms and Tamina's services. By connecting to this MCP server, AI assistants can access Tamina's functionality directly during your conversations and development sessions. The server is hosted at **https://tamina.app/api/mcp** and requires authentication before use.

## Prerequisites

Before connecting to the Tamina MCP server, you need:

- An active account on [Tamina](https://tamina.app)
- Valid authentication credentials from your Tamina account
- An AI platform that supports MCP (Model Context Protocol)

## Connecting to ChatGPT

To connect the Tamina MCP server to ChatGPT:

1. Open ChatGPT and navigate to your settings.
2. Look for the "Integrations" or "MCP Servers" section in the settings menu.
3. Click on "Add MCP Server" or "Connect New Server".
4. Enter the server URL: `https://tamina.app/api/mcp`
5. When prompted, provide your Tamina authentication credentials.
6. Save the configuration to establish the connection.
7. Once connected, ChatGPT will be able to access Tamina's capabilities through the MCP protocol.

## Connecting to Claude

To connect the Tamina MCP server to Claude (Anthropic):

1. Open Claude Desktop or Claude in your browser.
2. Navigate to the settings menu (typically found in the top-right corner).
3. Select "MCP Servers" or "External Integrations" from the settings options.
4. Click "Add Server" or "New MCP Connection".
5. In the server URL field, enter: `https://tamina.app/api/mcp`
6. Provide your Tamina authentication credentials when requested.
7. Confirm and save the configuration.
8. Claude will now have access to Tamina's services through the MCP connection.

## Connecting to GitHub Copilot

To connect the Tamina MCP server to GitHub Copilot:

1. Open Visual Studio Code or your preferred IDE with GitHub Copilot installed.
2. Access the GitHub Copilot settings through the command palette (Ctrl+Shift+P or Cmd+Shift+P).
3. Search for "MCP" or "Model Context Protocol" settings.
4. Select "Add MCP Server" or "Configure External Servers".
5. Enter the server URL: `https://tamina.app/api/mcp`
6. Input your Tamina authentication credentials when prompted.
7. Apply the settings and restart your IDE if necessary.
8. GitHub Copilot will now be able to utilize Tamina's functionality through the MCP connection.

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
