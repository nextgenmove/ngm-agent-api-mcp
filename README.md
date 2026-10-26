# Next Generation Movers MCP server

[![Listed on mcpservers.org](https://mcpservers.org/badge.svg)](https://mcpservers.org/servers/nextgenmove/ngm-agent-api) [![MCP](https://img.shields.io/badge/MCP-remote-blue)](https://ngm-agent-api.nextgenmovers.workers.dev/mcp) [![Glama](https://img.shields.io/badge/Glama-listed-green)](https://glama.ai/mcp/connectors/dev.workers.nextgenmovers.ngm-agent-api/movers) [![x402](https://img.shields.io/badge/x402-%240.01%20USDC-purple)](https://ngm-agent-api.nextgenmovers.workers.dev/)

Next Generation Movers is a licensed interstate household goods carrier (USDOT 3764697, MC 1341637), based at 645 Lofstrand Ln Unit B, Rockville, MD 20850.

This remote MCP server lets AI agents get moving quotes:

Version 0.6.1. Typical flow: `company_info` (optional), then `get_quote_free`, then `request_booking`.

- `get_quote_free`: free moving quote. Use this first. Optional contact fields send a callback lead to the owners; leave them out for a price only.
- `get_quote`: the same quote for $0.01 USDC via x402. Use it only when the free tool is rate-limited (30 per hour per IP) or your agent pays per call.
- `request_booking`: free date-hold request after a quote. Needs `move_date` plus `contact_email` or `contact_phone`.
- `company_info`: licensing, coverage, hours and contact. No inputs.

## Connect

Remote MCP endpoint (Streamable HTTP):

```
https://ngm-agent-api.nextgenmovers.workers.dev/mcp
```

## Docs

- For AI agents: https://nextgeneration-movers.com/for-ai-agents/
- llms.txt: https://ngm-agent-api.nextgenmovers.workers.dev/llms.txt
- OpenAPI: https://ngm-agent-api.nextgenmovers.workers.dev/openapi.json

## Contact

Phone: (240) 422-2243 · https://nextgeneration-movers.com/

This repo holds only the listing files. The server runs as a hosted service.

## Connect your agent

**Remote MCP:** `https://ngm-agent-api.nextgenmovers.workers.dev/mcp`  
**Agent card:** `https://ngm-agent-api.nextgenmovers.workers.dev/.well-known/agent.json`  
**Docs:** [For AI agents](https://nextgeneration-movers.com/for-ai-agents/) · [API llms.txt](https://ngm-agent-api.nextgenmovers.workers.dev/llms.txt)

Install: `npx add-mcp 'https://ngm-agent-api.nextgenmovers.workers.dev/mcp'`


- MCP endpoint (Streamable HTTP): `https://ngm-agent-api.nextgenmovers.workers.dev/mcp`
- Agent card: https://ngm-agent-api.nextgenmovers.workers.dev/.well-known/agent.json
- OpenAPI: https://ngm-agent-api.nextgenmovers.workers.dev/openapi.json
- llms.txt: https://ngm-agent-api.nextgenmovers.workers.dev/llms.txt

```json
{ "mcpServers": { "next-generation-movers": { "url": "https://ngm-agent-api.nextgenmovers.workers.dev/mcp" } } }
```
