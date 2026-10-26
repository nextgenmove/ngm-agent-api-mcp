# Next Generation Movers MCP server

Next Generation Movers is a licensed interstate household goods carrier (USDOT 3764697, MC 1341637), based at 645 Lofstrand Ln Unit B, Rockville, MD 20850.

This remote MCP server lets AI agents get moving quotes:

- `get_quote_free` – free moving quote (use this first)
- `get_quote` – the same quote, paid at $0.01 USDC via x402
- `request_booking` – free booking request
- `company_info` – licensing and contact details

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
