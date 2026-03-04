# Awesome MCP Servers [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Model Context Protocol (MCP) servers, tools, and resources.

[MCP](https://modelcontextprotocol.io/) is an open protocol that lets AI assistants connect to external data sources and tools. Think of it as USB-C for AI — one standard that works everywhere.

## Contents

- [Official](#official)
- [Server Frameworks](#server-frameworks)
- [Database Servers](#database-servers)
- [Developer Tools](#developer-tools)
- [Productivity](#productivity)
- [Communication](#communication)
- [Cloud & Infrastructure](#cloud--infrastructure)
- [File & Storage](#file--storage)
- [Search & Web](#search--web)
- [Data & Analytics](#data--analytics)
- [AI & ML](#ai--ml)
- [Finance](#finance)
- [Media](#media)
- [Security](#security)
- [Utilities](#utilities)
- [Client Libraries](#client-libraries)
- [Hosting & Deployment](#hosting--deployment)
- [Learning Resources](#learning-resources)

## Official

- [MCP Specification](https://spec.modelcontextprotocol.io/) - The official protocol specification.
- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) - Official TypeScript/Node.js SDK.
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk) - Official Python SDK.
- [MCP Servers](https://github.com/modelcontextprotocol/servers) - Reference server implementations by Anthropic.
- [MCP Inspector](https://github.com/modelcontextprotocol/inspector) - Visual testing tool for MCP servers.

## Server Frameworks

- [FastMCP](https://github.com/jlowin/fastmcp) - High-level Python framework for building MCP servers with decorators.
- [mcp-framework](https://github.com/QuantGeekDev/mcp-framework) - TypeScript framework for building MCP servers with CLI scaffolding.
- [EasyMCP](https://github.com/zueai/easymcp) - Simplified MCP server creation in TypeScript.
- [spring-ai-mcp](https://github.com/spring-projects-experimental/spring-ai-mcp) - Spring Boot integration for MCP servers.
- [mcp-rs](https://github.com/nicksenger/mcp-rs) - Rust SDK for building MCP servers.
- [go-mcp](https://github.com/mark3labs/mcp-go) - Go SDK for building MCP servers and clients.

## Database Servers

- [PostgreSQL MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) - Read-only PostgreSQL access with schema inspection.
- [SQLite MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) - SQLite database operations and analysis.
- [MySQL MCP](https://github.com/benborla/mcp-server-mysql) - MySQL/MariaDB database access.
- [MongoDB MCP](https://github.com/kiliczsh/mcp-mongo-server) - MongoDB collection operations.
- [Redis MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/redis) - Redis key-value operations.
- [Supabase MCP](https://github.com/supabase-community/supabase-mcp) - Supabase database and storage access.
- [Pinecone MCP](https://github.com/pinecone-io/pinecone-mcp) - Vector database operations with Pinecone.
- [Qdrant MCP](https://github.com/qdrant/mcp-server-qdrant) - Qdrant vector database integration.
- [Neo4j MCP](https://github.com/neo4j-contrib/mcp-neo4j) - Neo4j graph database queries.
- [Elasticsearch MCP](https://github.com/cr7258/elasticsearch-mcp-server) - Elasticsearch search and indexing.

## Developer Tools

- [GitHub MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/github) - GitHub API for repos, issues, PRs, and more.
- [GitLab MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/gitlab) - GitLab API integration.
- [Git MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/git) - Local git repository operations.
- [Docker MCP](https://github.com/ckreiling/mcp-server-docker) - Docker container and image management.
- [Kubernetes MCP](https://github.com/strowk/mcp-k8s-go) - Kubernetes cluster management.
- [Terraform MCP](https://github.com/hashicorp/terraform-mcp-server) - Terraform infrastructure management.
- [Sentry MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/sentry) - Error tracking and monitoring.
- [Linear MCP](https://github.com/jerhadf/linear-mcp-server) - Linear issue tracking integration.
- [Jira MCP](https://github.com/sooperset/mcp-atlassian) - Jira and Confluence integration.
- [Playwright MCP](https://github.com/executeautomation/mcp-playwright) - Browser automation for testing.

## Productivity

- [Google Drive MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/gdrive) - Google Drive file search and access.
- [Google Calendar MCP](https://github.com/nspaeth/google-calendar-mcp) - Google Calendar event management.
- [Notion MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/notion) - Notion workspace access.
- [Obsidian MCP](https://github.com/smithery-ai/mcp-obsidian) - Obsidian vault management.
- [Todoist MCP](https://github.com/abhiz123/todoist-mcp-server) - Todoist task management.
- [Apple Notes MCP](https://github.com/Dhravya/apple-mcp) - Apple Notes, Reminders, and Contacts.
- [Airtable MCP](https://github.com/felores/airtable-mcp) - Airtable base operations.
- [Trello MCP](https://github.com/tomdyson/mcp-trello) - Trello board management.

## Communication

- [Slack MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) - Slack workspace integration.
- [Discord MCP](https://github.com/v-gar/mcp-discord) - Discord bot and channel management.
- [Email MCP](https://github.com/baryhuang/mcp-server-email) - Email sending via SMTP.
- [Telegram MCP](https://github.com/nicholasgasior/mcp-telegram) - Telegram messaging.
- [WhatsApp MCP](https://github.com/lharris42/mcp-whatsapp) - WhatsApp messaging via WhatsApp Web.
- [Microsoft Teams MCP](https://github.com/modelcontextprotocol/servers) - Teams integration.

## Cloud & Infrastructure

- [AWS MCP](https://github.com/rishikavikondala/mcp-server-aws) - AWS service operations.
- [Azure MCP](https://github.com/mashriram/azure-mcp) - Azure resource management.
- [GCP MCP](https://github.com/nicholascelesmo/mcp-gcp) - Google Cloud Platform operations.
- [Cloudflare MCP](https://github.com/cloudflare/mcp-server-cloudflare) - Cloudflare service management.
- [Vercel MCP](https://github.com/vercel/mcp) - Vercel deployment management.
- [Firebase MCP](https://github.com/nicholascelesmo/mcp-firebase) - Firebase operations.
- [DigitalOcean MCP](https://github.com/digitalocean/mcp-server) - DigitalOcean resource management.

## File & Storage

- [Filesystem MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) - Local file system operations with security.
- [S3 MCP](https://github.com/aws/mcp-server-s3) - AWS S3 bucket operations.
- [Google Cloud Storage MCP](https://github.com/nicholascelesmo/mcp-gcs) - GCS bucket operations.
- [FTP MCP](https://github.com/apify/mcp-server-ftp) - FTP/SFTP file operations.

## Search & Web

- [Brave Search MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) - Brave web search API.
- [Google Search MCP](https://github.com/nicholasgasior/mcp-googlesearch) - Google Custom Search integration.
- [Exa MCP](https://github.com/exa-labs/exa-mcp-server) - Neural search with Exa API.
- [Fetch MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) - Web page fetching and conversion.
- [Puppeteer MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) - Headless browser automation.
- [Firecrawl MCP](https://github.com/mendableai/firecrawl-mcp-server) - Advanced web scraping and crawling.
- [Tavily MCP](https://github.com/RamXX/mcp-tavily) - AI-optimized search.

## Data & Analytics

- [BigQuery MCP](https://github.com/LucasHild/mcp-server-bigquery) - Google BigQuery queries.
- [Snowflake MCP](https://github.com/datawiz168/mcp-snowflake) - Snowflake data warehouse access.
- [PostHog MCP](https://github.com/PostHog/posthog-mcp) - Product analytics queries.
- [Datadog MCP](https://github.com/winor30/mcp-server-datadog) - Monitoring and metrics.
- [Grafana MCP](https://github.com/grafana/mcp-grafana) - Dashboard and alerting.

## AI & ML

- [OpenAI MCP](https://github.com/nicholasgasior/mcp-openai) - OpenAI API integration.
- [Anthropic MCP](https://github.com/anthropics/anthropic-mcp) - Anthropic Claude API access.
- [Ollama MCP](https://github.com/pamellix/ollama-mcp-server) - Local Ollama model inference.
- [Hugging Face MCP](https://github.com/huggingface/mcp-hf) - Hugging Face model and dataset access.
- [Replicate MCP](https://github.com/deepfates/mcp-replicate) - Replicate model inference.
- [LangChain MCP](https://github.com/langchain-ai/langchain-mcp) - LangChain tool integration.

## Finance

- [Stripe MCP](https://github.com/stripe/agent-toolkit) - Stripe payment operations.
- [Coinbase MCP](https://github.com/coinbase/cdp-agentkit) - Crypto wallet and trading.
- [Plaid MCP](https://github.com/plaid/mcp-server-plaid) - Banking data access.
- [Yahoo Finance MCP](https://github.com/akacdev/mcp-yahoo-finance) - Stock market data.

## Media

- [YouTube MCP](https://github.com/nicholasgasior/mcp-youtube) - YouTube video data and transcripts.
- [Spotify MCP](https://github.com/varunneal/spotify-mcp) - Spotify playback and library.
- [Image Generation MCP](https://github.com/modelcontextprotocol/servers) - AI image generation.
- [FFmpeg MCP](https://github.com/damianvalle/mcp-server-ffmpeg) - Video/audio processing.

## Security

- [Snyk MCP](https://github.com/snyk/mcp-server-snyk) - Vulnerability scanning.
- [Vault MCP](https://github.com/hashicorp/vault-mcp) - HashiCorp Vault secrets.
- [1Password MCP](https://github.com/1Password/mcp-server-1password) - 1Password secret management.

## Utilities

- [Time MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/time) - Time zones and conversions.
- [Weather MCP](https://github.com/modelcontextprotocol/servers/tree/main/src/weather) - Weather forecasts via NWS.
- [Calculator MCP](https://github.com/modelcontextprotocol/servers) - Mathematical computations.
- [QR Code MCP](https://github.com/jiaqi-yin/mcp-server-qrcode) - QR code generation.
- [Shell MCP](https://github.com/nicholasgasior/mcp-shell) - System shell command execution.

## Client Libraries

- [MCP TypeScript Client](https://github.com/modelcontextprotocol/typescript-sdk) - TypeScript/Node.js client.
- [MCP Python Client](https://github.com/modelcontextprotocol/python-sdk) - Python client.
- [MCP Go Client](https://github.com/mark3labs/mcp-go) - Go client library.
- [MCP Rust Client](https://github.com/nicksenger/mcp-rs) - Rust client library.
- [MCP Swift Client](https://github.com/modelcontextprotocol/swift-sdk) - Swift client for iOS/macOS.
- [MCP Kotlin Client](https://github.com/modelcontextprotocol/kotlin-sdk) - Kotlin/JVM client.

## Hosting & Deployment

- [Smithery](https://smithery.ai/) - Registry and hosting platform for MCP servers.
- [Glama](https://glama.ai/mcp/servers) - MCP server directory and hosting.
- [mcp-get](https://github.com/michaellatman/mcp-get) - Package manager for MCP servers.
- [mcpx](https://github.com/punkpeye/mcpx) - MCP server runner and manager.

## Learning Resources

- [MCP Documentation](https://modelcontextprotocol.io/docs) - Official documentation.
- [Building MCP Servers](https://modelcontextprotocol.io/tutorials/building-a-server) - Step-by-step tutorial.
- [MCP Examples](https://github.com/modelcontextprotocol/servers) - Reference implementations.
- [Awesome MCP Clients](https://github.com/punkpeye/awesome-mcp-clients) - MCP client applications.

---

## Contributing

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## License

[MIT](LICENSE)
