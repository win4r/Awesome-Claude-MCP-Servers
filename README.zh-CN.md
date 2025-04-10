# Claude MCP 服务器精选 🤖 [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[English](./README.md) | 中文版

## 目录
- [关于 MCP](#关于-mcp)
- [入门指南](#入门指南)
- [核心服务器](#核心服务器)
- [扩展功能](#扩展功能)
- [开发工具](#开发工具)
- [社区资源](#社区资源)

## 关于 MCP

[模型上下文协议（MCP）](https://modelcontextprotocol.io/)是一个开放协议，使 Claude 等 AI 模型能够通过标准化服务器实现安全地与本地和远程资源交互。这些服务器通过文件访问、数据库连接、API 集成和其他上下文服务扩展 Claude 的功能。

## 入门指南

- 📚 [模型上下文协议（MCP）快速入门](https://glama.ai/blog/2024-11-25-model-context-protocol-quickstart)
- 💬 [Discord 社区](https://discord.gg/TFE8FmjCdS)

## 图例

🏆 官方实现 | 🐍 Python | 📱 TypeScript | 🏃 Go | ☁️ 云服务 | 🏠 本地服务

## 核心服务器

### 文件系统 📂
安全访问和管理本地及云存储系统中的文件。

- [@modelcontextprotocol/server-filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) 📱 🏠 - 具有可配置权限的本地文件系统操作
- [@modelcontextprotocol/server-google-drive](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive) 📱 ☁️ - Google Drive 文件管理集成
- [mark3labs/mcp-filesystem-server](https://github.com/mark3labs/mcp-filesystem-server) 🏃 🏠 - 基于 Go 的本地文件访问实现

### 搜索引擎 🔍
访问实时网络信息和专业搜索功能。

- [exa-labs/exa-mcp-server](https://github.com/exa-labs/exa-mcp-server) 🏆 📱 ☁️ - 使用 Exa AI 搜索 API 的实时网络搜索
- [@modelcontextprotocol/server-brave-search](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) 📱 ☁️ - 通过 Brave 搜索 API 进行网络搜索
- [ac3xx/mcp-servers-kagi](https://github.com/ac3xx/mcp-servers-kagi) 📱 ☁️ - Kagi 搜索引擎集成
- [blazickjp/arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server) 🐍 ☁️ - 通过 ArXiv 搜索研究论文

### 数据库 🗄️
在保持安全的同时查询和分析数据。

- [@modelcontextprotocol/server-postgres](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) 📱 🏠 - PostgreSQL 集成及架构检查
- [@modelcontextprotocol/server-sqlite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) 🐍 🏠 - 具有分析功能的 SQLite 操作

## 扩展功能

### 知识与记忆 🧠
跨会话维护上下文和信息。

- [@modelcontextprotocol/server-memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) 📱 🏠 - 基于知识图谱的持久记忆系统

### 版本控制 📊
管理代码仓库和开发工作流。

- [@modelcontextprotocol/server-github](https://github.com/modelcontextprotocol/servers/tree/main/src/github) 📱 ☁️ - GitHub 仓库和问题集成
- [@modelcontextprotocol/server-gitlab](https://github.com/modelcontextprotocol/servers/tree/main/src/gitlab) 📱 ☁️ - GitLab 平台管理
- [@modelcontextprotocol/server-git](https://github.com/modelcontextprotocol/servers/tree/main/src/git) 🐍 🏠 - 直接 Git 仓库操作

### 云集成 ☁️
与云基础设施服务交互。

- [Cloudflare MCP Server](https://github.com/cloudflare/mcp-server-cloudflare) 🏆 📱 ☁️ - 访问 Cloudflare 服务，包括 Workers 和 KV

### 通信 💬
集成团队通信平台。

- [@modelcontextprotocol/server-slack](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) 📱 ☁️ - Slack 工作区和频道管理

### 浏览器自动化 🌐
以编程方式访问和处理网页内容。

- [@modelcontextprotocol/server-puppeteer](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) 📱 🏠 - 网页自动化和抓取
- [@modelcontextprotocol/server-youtube](https://github.com/kimtaeyoon83/mcp-server-youtube-transcript) 📱 ☁️ - YouTube 字幕提取

### 位置服务 🗺️
访问地理和地图数据。

- [@modelcontextprotocol/server-google-maps](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps) 📱 ☁️ - 地图集成用于位置和路线规划

### 监控 📈
跟踪应用程序性能和错误。

- [@modelcontextprotocol/server-sentry](https://github.com/modelcontextprotocol/servers/tree/main/src/sentry) 🐍 ☁️ - 通过 Sentry.io 进行错误跟踪
- [@modelcontextprotocol/server-raygun](https://github.com/MindscapeHQ/mcp-server-raygun) 📱 ☁️ - 通过 Raygun 进行崩溃报告

## 开发工具

### 框架 🛠️
用于构建和扩展 MCP 功能的工具。

- [Genkit MCP](https://github.com/firebase/genkit/tree/main/js/plugins/mcp) 📱 - Genkit 和 MCP 的集成
- [@modelcontextprotocol/server-langchain](https://github.com/rectalogic/langchain-mcp) 🐍 - MCP 工具的 LangChain 集成
- [mark3labs/mcp-go](https://github.com/mark3labs/mcp-go) 🏃 - MCP 开发的 Go SDK
- [TencentEdgeOne/edgeone-pages-mcp](https://github.com/TencentEdgeOne/edgeone-pages-mcp) 🐍 🏠 - EdgeOne Pages 集成 MCP 快捷生成在线网页

### 集成工具 🔧
针对特定平台和用例的专用工具。

- [pierrebrunelle/mcp-server-openai](https://github.com/pierrebrunelle/mcp-server-openai) 🐍 ☁️ - OpenAI 模型集成
- [@modelcontextprotocol/server-everything](https://github.com/modelcontextprotocol/servers/tree/main/src/everything) 📱 🏠 - 全面的 MCP 功能测试
- [calclavia/mcp-obsidian](https://github.com/calclavia/mcp-obsidian) 📱 🏠 - Obsidian 知识库集成
- [rusiaaman/wcgw](https://github.com/rusiaaman/wcgw/blob/main/src/wcgw/client/mcp_server/Readme.md) 🐍 🏠 - Shell 执行和计算机控制

## 社区资源

想要向 Claude 询问模型上下文协议？将此文件添加到您的项目中：
[Claude MCP 说明](https://raw.githubusercontent.com/win4r/Awesome-Claude-MCP-Servers/refs/heads/main/llms-full.txt)
