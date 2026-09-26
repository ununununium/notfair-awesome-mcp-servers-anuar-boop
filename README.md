# Awesome MCP Servers [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) servers, frameworks, SDKs, and resources.

The **Model Context Protocol** is an open standard created by [Anthropic](https://www.anthropic.com/news/model-context-protocol) that enables AI assistants to securely connect to external tools, data sources, and services through a unified interface. Think of it as a USB-C port for AI — one protocol to connect any model to any tool.

MCP follows a client-server architecture where AI applications (clients) connect to MCP servers that expose tools, resources, and prompts. This decouples the AI model from the integrations, making it possible to mix and match any model with any tool.

**How it works:** AI Host (Claude, Cursor, VS Code) &rarr; MCP Client &rarr; MCP Server &rarr; External Service (API, database, filesystem, etc.)

---

## Contents

- [Official Servers](#official-servers)
- [Development Tools](#development-tools)
- [Database & Data](#database--data)
- [Cloud & Infrastructure](#cloud--infrastructure)
- [Communication](#communication)
- [Search & Web](#search--web)
- [AI & ML](#ai--ml)
- [File & Storage](#file--storage)
- [Monitoring & Observability](#monitoring--observability)
- [Security](#security)
- [Frameworks & SDKs](#frameworks--sdks)
- [Resources](#resources)

---

## Official Servers

Reference implementations maintained by the [MCP organization](https://github.com/modelcontextprotocol) and Anthropic.

- [Filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) — Secure file operations with configurable access controls and directory sandboxing.
- [Git](https://github.com/modelcontextprotocol/servers/tree/main/src/git) — Tools to read, search, and manipulate Git repositories including diffs, logs, and branch management.
- [Memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) — Knowledge graph-based persistent memory system for maintaining context across sessions.
- [Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) — Web content fetching and conversion optimized for efficient LLM consumption.
- [Sequential Thinking](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) — Dynamic and reflective problem-solving through structured thought sequences.
- [Everything](https://github.com/modelcontextprotocol/servers/tree/main/src/everything) — Reference/test server demonstrating all MCP capabilities including prompts, resources, and tools.
- [Time](https://github.com/modelcontextprotocol/servers/tree/main/src/time) — Time and timezone conversion capabilities for scheduling and coordination tasks.
- [PostgreSQL](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/postgres) — Read-only PostgreSQL database access with schema inspection. *(Archived)*
- [SQLite](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/sqlite) — SQLite database operations including queries, analysis, and business intelligence. *(Archived)*
- [Puppeteer](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/puppeteer) — Browser automation for web scraping, screenshots, and interaction. *(Archived)*
- [Brave Search](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/brave-search) — Web and local search via the Brave Search API. *(Archived)*
- [GitHub](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/github) — GitHub API integration for repos, issues, PRs, and file operations. *(Archived)*
- [Google Maps](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/google-maps) — Location services, directions, and place details from Google Maps. *(Archived)*
- [Slack](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/slack) — Slack workspace integration for channels, messages, and user management. *(Archived)*
- [Google Drive](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/gdrive) — File access and search across Google Drive. *(Archived)*
- [Sentry](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/sentry) — Error tracking and issue retrieval from Sentry projects. *(Archived)*

> **Note:** Several official servers have been archived and moved to community or vendor maintenance. They remain functional but are no longer updated by the MCP steering group.

## Development Tools

IDE integrations, code analysis, debugging, and testing servers.

- [JetBrains MCP](https://github.com/JetBrains/mcp-jetbrains) — MCP server for all JetBrains IDEs (IntelliJ, PyCharm, WebStorm, Android Studio) with code analysis, refactoring, and project tools.
- [Playwright MCP](https://github.com/microsoft/playwright-mcp) — Official Microsoft Playwright server for browser automation, end-to-end testing, and web scraping.
- [Docker MCP](https://github.com/docker/docker-mcp) — Docker container management, image operations, and Compose workflows.
- [Linear MCP](https://github.com/linear/linear-mcp) — Project management integration with Linear for issues, projects, and workflow automation.
- [Jira & Confluence MCP](https://github.com/sooperset/mcp-atlassian) — Atlassian Jira and Confluence integration for issue tracking and documentation.
- [Desktop Commander](https://github.com/wonderwhy-er/DesktopCommanderMCP) — Terminal command execution, file operations, and diff-based editing for AI coding agents.
- [Semgrep MCP](https://github.com/semgrep/mcp) — Static analysis and code scanning using Semgrep rules for security and quality.
- [Sourcegraph MCP](https://sourcegraph.com/docs/cody/mcp) — Code intelligence and cross-repository search through Sourcegraph's code graph.
- [GitKraken MCP](https://help.gitkraken.com/mcp/mcp-getting-started/) — Git operations and repository management through the GitKraken platform.
- [Jupyter MCP](https://github.com/datalayer/jupyter-mcp-server) — Jupyter notebook execution, cell management, and kernel interaction.
- [Nx MCP](https://github.com/nrwl/nx-mcp) — Nx monorepo tooling for project graph analysis, task running, and workspace management.
- [Postman MCP](https://github.com/nicepkg/aide) — API testing and collection management through Postman.

## Database & Data

Database connectors, query tools, and data platform integrations.

- [MySQL MCP](https://github.com/designcomputer/mysql_mcp_server) — MySQL database integration with configurable access controls, schema inspection, and query execution.
- [MongoDB MCP](https://github.com/kiliczsh/mcp-mongo-server) — MongoDB operations including CRUD, aggregation pipelines, and collection management.
- [Redis MCP](https://github.com/redis/mcp-redis) — Official Redis server for data management, caching, and vector search operations.
- [Supabase MCP](https://github.com/supabase-community/supabase-mcp) — Supabase integration for Postgres queries, edge functions, storage, and authentication.
- [PlanetScale MCP](https://github.com/planetscale/mcp-server) — PlanetScale serverless MySQL with branch management and schema migrations.
- [Pinecone MCP](https://github.com/pinecone-io/pinecone-mcp) — Official Pinecone vector database server for similarity search, upserts, and index management.
- [Weaviate MCP](https://github.com/weaviate/mcp-server-weaviate) — Weaviate vector database for knowledge base access and chat memory storage.
- [Qdrant MCP](https://github.com/qdrant/mcp-server-qdrant) — Qdrant vector search engine integration for embeddings, collections, and semantic retrieval.
- [Neon MCP](https://github.com/neondatabase/mcp-server-neon) — Neon serverless Postgres with branching, connection pooling, and database management.
- [SQLAlchemy MCP](https://github.com/runekaagaard/mcp-alchemy) — Universal database integration via SQLAlchemy supporting PostgreSQL, MySQL, MariaDB, SQLite, Oracle, and MS SQL.
- [ClickHouse MCP](https://github.com/ClickHouse/mcp-clickhouse) — ClickHouse analytical database queries, schema exploration, and data analysis.
- [Neo4j MCP](https://github.com/neo4j-contrib/mcp-neo4j) — Neo4j graph database queries, Cypher execution, and relationship traversal.

## Cloud & Infrastructure

Cloud platform management, container orchestration, and infrastructure-as-code tools.

- [AWS MCP](https://github.com/awslabs/mcp) — Official AWS integration supporting Lambda, ECS, EKS, S3, EC2, RDS, CloudWatch, and cost analytics.
- [Azure MCP](https://github.com/Azure/azure-mcp) — Microsoft Azure services including RBAC configuration, Azure Monitor logs, Cosmos DB, and resource management.
- [Google Cloud MCP](https://github.com/GoogleCloudPlatform/mcp-server) — GCP integration for Compute Engine, Cloud Storage, BigQuery, and Cloud Run.
- [Cloudflare MCP](https://github.com/cloudflare/mcp-server-cloudflare) — Cloudflare Workers, KV, R2 storage, D1 databases, and DNS management.
- [Terraform MCP](https://github.com/hashicorp/terraform-mcp-server) — Official HashiCorp Terraform integration for IaC development, registry access, and provider documentation.
- [Kubernetes MCP](https://github.com/flux159/mcp-server-kubernetes) — Kubernetes cluster management including pods, deployments, services, and namespace operations.
- [Pulumi MCP](https://github.com/pulumi/mcp-server) — Pulumi infrastructure-as-code for multi-cloud deployments with state management.
- [LocalStack MCP](https://github.com/localstack/localstack-mcp-server) — Local AWS environment management for development and testing without cloud costs.
- [Vercel MCP](https://github.com/vercel/mcp) — Vercel deployment management, project configuration, and serverless function operations.
- [Alibaba Cloud MCP](https://github.com/aliyun/alibaba-cloud-ops-mcp-server) — Alibaba Cloud operations for ECS, OSS, RDS, and cloud resource management.
- [Kestra MCP](https://github.com/kestra-io/mcp-server-python) — Kestra workflow orchestration for data pipelines, scheduling, and event-driven automation.
- [Netlify MCP](https://github.com/netlify/mcp-server-netlify) — Netlify site management, deployments, build configuration, and serverless functions.

## Communication

Messaging platforms, email, calendar, and productivity tool integrations.

- [Slack MCP](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/slack) — Slack workspace operations including channel management, messaging, and user lookups.
- [Discord MCP](https://github.com/v-3/discordmcp) — Discord bot integration for server management, messaging, and channel operations.
- [Notion MCP](https://github.com/makenotion/notion-mcp-server) — Notion workspace integration for pages, databases, and content management.
- [Google Calendar MCP](https://github.com/nspady/google-calendar-mcp) — Google Calendar event management, scheduling, and availability checking.
- [Linear MCP](https://github.com/linear/linear-mcp) — Linear issue tracking, project management, and cycle planning.
- [Jira MCP](https://github.com/sooperset/mcp-atlassian) — Atlassian Jira and Confluence integration for issue tracking and documentation.
- [Resend MCP](https://github.com/resend/mcp-server) — Transactional email sending via the Resend API with template support.
- [Twilio MCP](https://github.com/twilio/mcp-server) — SMS, voice, and communication APIs through Twilio's platform.
- [Todoist MCP](https://github.com/abhiz123/todoist-mcp-server) — Todoist task management for creating, updating, and organizing tasks and projects.
- [Apple Notes MCP](https://github.com/Dhravya/apple-mcp) — Apple Notes, Reminders, and Contacts access on macOS.
- [Telegram MCP](https://github.com/nicholasgasior/mcp-telegram) — Telegram messaging and bot interactions.
- [WhatsApp MCP](https://github.com/lharris42/mcp-whatsapp) — WhatsApp messaging via the WhatsApp Web protocol.

## Search & Web

Web scraping, search engines, and API integrations.

- [Brave Search MCP](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/brave-search) — Web and local search using the Brave Search API with privacy focus.
- [Firecrawl MCP](https://github.com/mendableai/firecrawl-mcp-server) — Web scraping and crawling with automatic content extraction and markdown conversion.
- [Exa MCP](https://github.com/exa-labs/exa-mcp-server) — Neural search engine for finding semantically relevant web content and research.
- [Tavily MCP](https://github.com/tavily-ai/tavily-mcp) — AI-optimized search API designed for LLM applications with fact-checking capabilities.
- [Browserbase MCP](https://github.com/browserbase/mcp-server-browserbase) — Cloud browser automation for web scraping at scale with anti-detection.
- [Crawl4AI MCP](https://github.com/unclecode/crawl4ai) — Open-source web crawling optimized for AI with LLM-friendly output formats.
- [Algolia MCP](https://github.com/algolia/mcp-server) — Algolia search index management, queries, and analytics.
- [Apify MCP](https://github.com/apify/mcp-server-apify) — Access to 3,000+ web scraping and automation actors on the Apify platform.
- [Jina Reader MCP](https://github.com/jina-ai/reader-mcp) — Web page reading and content extraction using Jina AI's reader API.
- [SerpAPI MCP](https://github.com/nicepkg/aide) — Google search results, knowledge graph, and SERP data via SerpAPI.
- [Olostep MCP](https://github.com/olostep/olostep-mcp-server) — Web scraping and search API for structured data extraction from any website.
- [Perplexity MCP](https://github.com/nicepkg/aide) — Perplexity AI search integration for research and question answering.
- [Statsnet MCP](https://github.com/usenetstate/statsnet-mcp) — Background check any company in the world: registration, executives, courts and finances. Remote: `https://statsnet.co/mcp`.

## AI & ML

Model management, vector stores, embedding tools, and AI service integrations.

- [OpenAI MCP](https://github.com/nicepkg/aide) — OpenAI API integration for GPT models, embeddings, DALL-E image generation, and assistants.
- [Ollama MCP](https://github.com/ollama/ollama-mcp) — Local LLM inference through Ollama for private, offline model execution.
- [HuggingFace MCP](https://github.com/huggingface/mcp-server) — HuggingFace Hub access for model discovery, dataset browsing, and inference API.
- [LangChain MCP Adapters](https://github.com/langchain-ai/langchain-mcp-adapters) — Adapters to use MCP tools within LangChain and LangGraph agent workflows.
- [Weights & Biases MCP](https://github.com/wandb/mcp-server) — Experiment tracking, model registry, and artifact management through W&B.
- [ChromaDB MCP](https://github.com/chroma-core/chroma-mcp) — ChromaDB vector database for embedding storage, similarity search, and RAG applications.
- [MindsDB MCP](https://github.com/mindsdb/mindsdb) — AI data platform unifying databases with ML models for predictions and automation.
- [Replicate MCP](https://github.com/deepfates/mcp-replicate) — Run open-source ML models in the cloud via Replicate's inference platform.
- [Cohere MCP](https://github.com/cohere-ai/mcp-server) — Cohere language models for embeddings, reranking, and retrieval-augmented generation.
- [AgentOps MCP](https://github.com/AgentOps-AI/agentops-mcp) — AI agent observability with session tracking, cost monitoring, and debugging.
- [Gemini MCP](https://github.com/nicepkg/aide) — Google Gemini API bridge for multimodal AI capabilities.
- [fal.ai MCP](https://github.com/raveenb/fal-mcp-server) — AI image, video, and music generation via fal.ai's inference platform.

## File & Storage

File systems, cloud storage, and document management.

- [Filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) — Secure local file operations with configurable access controls and sandboxing.
- [Google Drive MCP](https://github.com/modelcontextprotocol/servers-archived/tree/main/src/gdrive) — Google Drive file access, search, and document management.
- [S3 MCP](https://github.com/awslabs/mcp) — Amazon S3 bucket operations including file upload, download, listing, and management.
- [Box MCP](https://github.com/box/mcp-server-box) — Box content management for enterprise file operations and collaboration.
- [R2 MCP](https://github.com/cloudflare/mcp-server-cloudflare) — Cloudflare R2 object storage for S3-compatible file operations.
- [MinIO MCP](https://github.com/minio/mcp-server-minio) — MinIO self-hosted object storage for private cloud file management.
- [Obsidian MCP](https://github.com/smithery-ai/mcp-obsidian) — Obsidian vault management for note access, search, and knowledge graph traversal.
- [Pandoc MCP](https://github.com/vivekVells/mcp-pandoc) — Document format conversion between Markdown, HTML, PDF, DOCX, and more using Pandoc.
- [Dropbox MCP](https://github.com/nicepkg/aide) — Dropbox file synchronization, sharing, and folder management.
- [OneDrive MCP](https://github.com/nicepkg/aide) — Microsoft OneDrive and SharePoint file access and management.
- [Airtable MCP](https://github.com/felores/airtable-mcp) — Airtable base operations for structured data and spreadsheet-like management.

## Monitoring & Observability

Logging, metrics, alerting, and system health tools.

- [Datadog MCP](https://github.com/shelfio/datadog-mcp) — Comprehensive Datadog monitoring with dashboards, logs, metrics, APM, and security scanning.
- [Grafana MCP](https://grafana.com/docs/grafana-cloud/monitor-applications/ai-observability/mcp-observability/) — Grafana dashboards, alerting, and MCP-specific observability for protocol health monitoring.
- [Sentry MCP](https://github.com/getsentry/sentry-mcp) — Sentry error tracking, issue management, and performance monitoring for applications.
- [PagerDuty MCP](https://github.com/nicepkg/aide) — PagerDuty incident management, on-call schedules, and alert routing.
- [Prometheus MCP](https://github.com/nicepkg/aide) — Prometheus metrics querying with PromQL, alert rules, and time series analysis.
- [Axiom MCP](https://github.com/axiomhq/mcp-server-axiom) — Axiom log management with APL queries for fast log analysis and exploration.
- [Elastic MCP](https://github.com/elastic/mcp-server-elasticsearch) — Elasticsearch and Kibana integration for log search, aggregations, and analytics.
- [CloudWatch MCP](https://github.com/awslabs/mcp) — AWS CloudWatch metrics, log groups, alarms, and dashboard management.
- [Checkly MCP](https://github.com/checkly/mcp-server) — Checkly synthetic monitoring, API checks, and browser check management.
- [PostHog MCP](https://github.com/PostHog/posthog-mcp) — PostHog product analytics, feature flags, and session replay queries.
- [BetterStack MCP](https://github.com/nicepkg/aide) — BetterStack uptime monitoring, status pages, and incident management.

## Security

Secret management, authentication, vulnerability scanning, and compliance tools.

- [1Password MCP](https://github.com/1Password/mcp-server-1password) — 1Password vault access for secret retrieval and credential management.
- [Vault MCP](https://github.com/hashicorp/vault-mcp-server) — HashiCorp Vault integration for secrets, encryption, and identity-based access.
- [Snyk MCP](https://github.com/snyk/mcp-server) — Snyk vulnerability scanning for open-source dependencies and container images.
- [Auth0 MCP](https://github.com/auth0/auth0-mcp-server) — Auth0 identity management for user authentication, roles, and permissions.
- [CrowdStrike MCP](https://github.com/crowdstrike/mcp-server) — CrowdStrike Falcon endpoint detection, threat intelligence, and incident response.
- [Trivy MCP](https://github.com/aquasecurity/trivy-mcp) — Aqua Trivy vulnerability scanner for containers, filesystems, and IaC misconfigurations.
- [Doppler MCP](https://github.com/dopplerhq/mcp-server) — Doppler secrets management for environment variables across projects and environments.
- [Tines MCP](https://github.com/tines/mcp-server) — Tines security orchestration and automated response (SOAR) workflows.
- [GitHub Security MCP](https://github.com/nicepkg/aide) — GitHub Advanced Security alerts, Dependabot, and code scanning results.
- [OWASP ZAP MCP](https://github.com/nicepkg/aide) — OWASP ZAP dynamic application security testing and vulnerability reports.

## Frameworks & SDKs

Official SDKs, server frameworks, and client libraries for building MCP integrations.

### Official SDKs

- [TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) — The official TypeScript/JavaScript SDK for building MCP servers and clients.
- [Python SDK](https://github.com/modelcontextprotocol/python-sdk) — The official Python SDK with async support and Pydantic validation.
- [Go SDK](https://github.com/modelcontextprotocol/go-sdk) — The official Go SDK maintained in collaboration with Google.
- [Rust SDK](https://github.com/modelcontextprotocol/rust-sdk) — The official Rust SDK with tokio async runtime integration.
- [Java SDK](https://github.com/modelcontextprotocol/java-sdk) — The official Java SDK for enterprise MCP server development.
- [Kotlin SDK](https://github.com/modelcontextprotocol/kotlin-sdk) — The official Kotlin SDK for JVM and Android MCP integrations.
- [C# SDK](https://github.com/modelcontextprotocol/csharp-sdk) — The official .NET SDK for building MCP servers in C# and F#.
- [Swift SDK](https://github.com/modelcontextprotocol/swift-sdk) — The official Swift SDK for macOS and iOS MCP development.

### Server Frameworks

- [FastMCP (Python)](https://github.com/jlowin/fastmcp) — The fast, Pythonic way to build MCP servers. Powers ~70% of MCP servers. Auto-generates schemas from decorated functions.
- [FastMCP (TypeScript)](https://github.com/punkpeye/fastmcp) — TypeScript framework for building MCP servers with session management, authentication, and streaming.
- [MCP-Framework](https://github.com/QuantGeekDev/mcp-framework) — TypeScript framework with class-based tools, resources, and CLI scaffolding.
- [FastAPI-MCP](https://github.com/tadata-ru/fastapi_mcp) — Expose any FastAPI application as an MCP server with zero code changes.
- [Foxy Contexts](https://github.com/nicepkg/aide) — High-performance Go framework for enterprise-grade MCP servers.
- [EasyMCP](https://github.com/zueai/easymcp) — Minimal TypeScript framework for building MCP servers with zero boilerplate.
- [Spring AI MCP](https://github.com/spring-projects-experimental/spring-ai-mcp) — Spring Boot integration for building MCP servers in the Java/Spring ecosystem.
- [Quarkus MCP](https://github.com/quarkiverse/quarkus-mcp-server) — Quarkus extension for building high-performance Java MCP servers with native compilation.

### Client Libraries & Tools

- [MCP Inspector](https://github.com/modelcontextprotocol/inspector) — Interactive developer tool for testing and debugging MCP servers.
- [mcp-get](https://github.com/michaellatman/mcp-get) — Package manager for installing and managing MCP servers.
- [Supergateway](https://github.com/nicepkg/aide) — Run stdio MCP servers over SSE or WebSocket for remote access.
- [MCP Proxy](https://github.com/nicepkg/aide) — Bridge between SSE and stdio transports for flexible MCP server deployment.

## Resources

Tutorials, documentation, blog posts, and community content.

### Official Documentation

- [MCP Specification](https://modelcontextprotocol.io/specification/2025-11-25) — The complete protocol specification with transport, capability, and message definitions.
- [MCP Documentation](https://modelcontextprotocol.io/) — Official docs covering quickstarts, concepts, and best practices.
- [Anthropic MCP Announcement](https://www.anthropic.com/news/model-context-protocol) — The original blog post introducing MCP to the world.
- [MCP GitHub Organization](https://github.com/modelcontextprotocol) — All official repositories including SDKs, servers, and the specification.

### Tutorials & Guides

- [Introduction to MCP (Anthropic Courses)](https://anthropic.skilljar.com/introduction-to-model-context-protocol) — Free official course covering MCP fundamentals and server development.
- [MCP Advanced Topics (Anthropic Courses)](https://anthropic.skilljar.com/model-context-protocol-advanced-topics) — Advanced course on production MCP deployments, security, and architecture.
- [Building MCP Servers with FastMCP (freeCodeCamp)](https://www.freecodecamp.org/news/how-to-build-your-first-mcp-server-using-fastmcp/) — Step-by-step guide to building your first MCP server in Python.
- [Understanding MCP (LogRocket)](https://blog.logrocket.com/understanding-anthropic-model-context-protocol-mcp/) — In-depth technical explainer of the protocol architecture and use cases.
- [Code Execution with MCP (Anthropic)](https://www.anthropic.com/engineering/code-execution-with-mcp) — Engineering deep dive on sandboxed code execution through MCP.

### Directories & Registries

- [MCP Server Registry](https://github.com/modelcontextprotocol/servers) — The official registry of reference and community MCP servers.
- [Awesome MCP Servers (punkpeye)](https://github.com/punkpeye/awesome-mcp-servers) — Community-maintained collection with 2,000+ servers organized by category.
- [Awesome MCP Servers (wong2)](https://github.com/wong2/awesome-mcp-servers) — Curated list focused on quality and practical use cases.
- [MCP.so](https://mcp.so) — Searchable web directory of MCP servers with ratings and reviews.
- [mcpservers.org](https://mcpservers.org/) — Community hub for discovering and sharing MCP servers.
- [Glama MCP Directory](https://glama.ai/mcp/servers) — Web-based MCP server directory with testing inspector.
- [PulseMCP](https://www.pulsemcp.com/) — MCP server discovery platform with detailed capability listings and usage guides.
- [Smithery](https://smithery.ai/) — Registry and hosting platform for MCP servers.

### Community

- [MCP Discord](https://discord.gg/modelcontextprotocol) — Official community Discord for discussion, support, and server showcases.
- [MCP Wikipedia](https://en.wikipedia.org/wiki/Model_Context_Protocol) — Wikipedia article covering the history and adoption of MCP.
- [Awesome MCP Clients](https://github.com/punkpeye/awesome-mcp-clients) — Companion list of MCP client applications.

---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

To add a new server:
1. Fork this repository
2. Add your entry to the appropriate category in `README.md`
3. Use the format: `[Name](url) — Description`
4. Keep descriptions concise (one sentence)
5. Submit a pull request

Quality standards:
- Server must be functional and documented
- Open-source projects preferred (include license)
- Commercial servers are welcome if they offer a free tier
- No duplicates of official reference servers

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the author has waived all copyright and related or neighboring rights to this work.
