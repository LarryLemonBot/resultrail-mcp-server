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

## Claim boundaries

- This repo is public metadata for a hosted remote MCP server, not a claim that private production source code is open source.
- Directory listings are discovery evidence only, not endorsement, certification, ranking, or security approval.

## License

Commercial hosted service metadata. All rights reserved unless a separate written license applies.