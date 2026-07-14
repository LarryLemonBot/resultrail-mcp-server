# ResultRail by LarryBuildsAI MCP Server

Public listing metadata for the hosted ResultRail by LarryBuildsAI remote MCP server.

This repository is intentionally metadata-only. The production MCP server is hosted remotely by LarryBuildsAI; private application source code, credentials, payment keys, and operator materials are not published here.

## Server

- Product: ResultRail by LarryBuildsAI
- Purpose: pay-per-success public-data result packs with source URLs, confidence, timestamps, and receipt hashes
- Remote MCP endpoint: `https://proofbeforepay.vercel.app/resultrail/mcp`
- Marketplace proof: `https://proofbeforepay.vercel.app/resultrail/marketplaces`
- Server card: `https://proofbeforepay.vercel.app/resultrail/.well-known/mcp/server-card.json`

## Install / connect

ResultRail is a remote Streamable HTTP MCP server. Use this endpoint in an MCP client that supports remote HTTP MCP servers:

```json
{
  "mcpServers": {
    "resultrail": {
      "url": "https://proofbeforepay.vercel.app/resultrail/mcp"
    }
  }
}
```

Public `initialize` and `tools/list` calls are available for discovery. Protected paid tool execution may require product-specific authorization and/or x402 payment flow.

## Buy through PayanAgent

PayanAgent validates buyer input, settles USDC, and returns the selected source-attributed result automatically:

- [Public domain result pack — $0.12](https://payanagent.com/marketplace/offers/kh7be0c7c7e51c11b65d31wtcd8ahdxd)
- [Public URL extract result — $0.05](https://payanagent.com/marketplace/offers/kh714wc600k8kdtj9h1kg0zjfd8ahpg1)

ResultRail reads public pages only and returns bounded source URLs, confidence, freshness, stop conditions, and deterministic result hashes. It does not access private data or credentials.

## Claim boundaries

- This repo is public metadata for a hosted remote MCP server, not a claim that private production source code is open source.
- Directory listings are discovery evidence only, not endorsement, certification, ranking, or security approval.

## License

Commercial hosted service metadata. All rights reserved unless a separate written license applies.
