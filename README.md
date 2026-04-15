# Awesome Claude MCP Servers 🤖 [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[中文版](./README.zh-CN.md) | English

A curated list of Model Context Protocol (MCP) servers optimized for Claude and other AI assistants.

## Contents
- [About MCP](#about-mcp)
- [Getting Started](#getting-started)
- [Core Servers](#core-servers)
- [Extended Capabilities](#extended-capabilities)
- [Development Tools](#development-tools)
- [Community Resources](#community-resources)

## About MCP

[Model Context Protocol (MCP)](https://modelcontextprotocol.io/) is an open protocol enabling AI models like Claude to securely interact with local and remote resources through standardized server implementations. These servers extend Claude's capabilities through file access, database connections, API integrations, and other contextual services.

## Getting Started

- 📚 [Model Context Protocol (MCP) Quickstart](https://glama.ai/blog/2024-11-25-model-context-protocol-quickstart)
- 💬 [Discord Community](https://discord.gg/TFE8FmjCdS)

## Legend

🏆 Official Implementation | 🐍 Python | 📱 TypeScript | 🏃 Go | ☁️ Cloud Service | 🏠 Local Service

## Core Servers

### File Systems 📂
Access and manage files securely across local and cloud storage systems.

- [@modelcontextprotocol/server-filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) 📱 🏠 - Local file system operations with configurable permissions
- [@modelcontextprotocol/server-google-drive](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive) 📱 ☁️ - Google Drive integration for file management
- [mark3labs/mcp-filesystem-server](https://github.com/mark3labs/mcp-filesystem-server) 🏃 🏠 - Go-based implementation for local file access

### Search Engines 🔍
Access real-time web information and specialized search capabilities.

- [exa-labs/exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) 🏆 📱 ☁️ - Real-time web search using Exa AI Search API
- [@modelcontextprotocol/server-brave-search](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) 📱 ☁️ - Web search via Brave's Search API
- [ac3xx/mcp-servers-kagi](https://github.com/ac3xx/mcp-servers-kagi) 📱 ☁️ - Integration with Kagi search engine
- [blazickjp/arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server) 🐍 ☁️ - Research paper search through ArXiv

### Databases 🗄️
Query and analyze data while maintaining security.

- [@modelcontextprotocol/server-postgres](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) 📱 🏠 - PostgreSQL integration with schema inspection
- [@modelcontextprotocol/server-sqlite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) 🐍 🏠 - SQLite operations with analysis features

## Extended Capabilities

### Knowledge & Memory 🧠
Maintain context and information across sessions.

- [@modelcontextprotocol/server-memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) 📱 🏠 - Knowledge graph-based persistent memory system

### Version Control 📊
Manage code repositories and development workflows.

- [@modelcontextprotocol/server-github](https://github.com/modelcontextprotocol/servers/tree/main/src/github) 📱 ☁️ - GitHub integration for repos and issues
- [@modelcontextprotocol/server-gitlab](https://github.com/modelcontextprotocol/servers/tree/main/src/gitlab) 📱 ☁️ - GitLab platform management
- [@modelcontextprotocol/server-git](https://github.com/modelcontextprotocol/servers/tree/main/src/git) 🐍 🏠 - Direct Git repository operations

### Cloud Integration ☁️
Interact with cloud infrastructure services.

- [Cloudflare MCP Server](https://github.com/cloudflare/mcp-server-cloudflare) 🏆 📱 ☁️ - Access to Cloudflare services including Workers and KV

### Communication 💬
Integrate with team communication platforms.

- [@modelcontextprotocol/server-slack](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) 📱 ☁️ - Slack workspace and channel management

### Browser Automation 🌐
Access and process web content programmatically.

- [@modelcontextprotocol/server-puppeteer](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) 📱 🏠 - Web automation and scraping
- [@modelcontextprotocol/server-youtube](https://github.com/kimtaeyoon83/mcp-server-youtube-transcript) 📱 ☁️ - YouTube subtitle extraction

### Location Services 🗺️
Access geographic and mapping data.

- [@modelcontextprotocol/server-google-maps](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) 📱 ☁️ - Maps integration for location and routing

### Monitoring 📈
Track application performance and errors.

- [@modelcontextprotocol/server-sentry](https://github.com/modelcontextprotocol/servers/tree/main/src/sentry) 🐍 ☁️ - Error tracking via Sentry.io
- [@modelcontextprotocol/server-raygun](https://github.com/MindscapeHQ/mcp-server-raygun) 📱 ☁️ - Crash reporting through Raygun


### Data & Business Intelligence 📊
Access business records, government data, and lead generation tools.

- [avabuildsdata/mcp-us-business-data](https://github.com/avabuildsdata/mcp-us-business-data) 🏃 ☁️ - US business entity search, Secretary of State filings, building permits, and Yellow Pages leads across 17 states

## Development Tools

### Frameworks 🛠️
Tools for building and extending MCP capabilities.

- [Genkit MCP](https://github.com/firebase/genkit/tree/main/js/plugins/mcp) 📱 - Integration between Genkit and MCP
- [@modelcontextprotocol/server-langchain](https://github.com/rectalogic/langchain-mcp) 🐍 - LangChain integration for MCP tools
- [mark3labs/mcp-go](https://github.com/mark3labs/mcp-go) 🏃 - Go SDK for MCP development

### Integration Tools 🔧
Specialized tools for specific platforms and use cases.

- [pierrebrunelle/mcp-server-openai](https://github.com/pierrebrunelle/mcp-server-openai) 🐍 ☁️ - OpenAI models integration
- [@modelcontextprotocol/server-everything](https://github.com/modelcontextprotocol/servers/tree/main/src/everything) 📱 🏠 - Comprehensive MCP feature testing
- [calclavia/mcp-obsidian](https://github.com/calclavia/mcp-obsidian) 📱 🏠 - Obsidian vault integration
- [rusiaaman/wcgw](https://github.com/rusiaaman/wcgw/blob/main/src/wcgw/client/mcp_server/Readme.md) 🐍 🏠 - Shell execution and computer control

## Community Resources

Want to ask Claude about Model Context Protocol? Add this file to your project:
[Claude MCP Instructions](https://raw.githubusercontent.com/win4r/Awesome-Claude-MCP-Servers/refs/heads/main/llms-full.txt)
