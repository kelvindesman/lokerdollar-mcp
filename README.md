# LokerDollar Jobs MCP Server

A free, anonymous, read-only [Model Context Protocol](https://modelcontextprotocol.io) server for searching remote jobs that pay in foreign currency, with an Indonesia and Southeast Asia focus.

- **Endpoint:** `https://mcp.lokerdollar.com/mcp`
- **Transport:** HTTP JSON-RPC 2.0 — `GET /mcp` returns a discovery manifest, no handshake required
- **Auth:** none. Fully anonymous, rate-limited per IP.
- **Tools:**
  - `search_jobs` — search by role, category, salary and remote eligibility
  - `get_job` — fetch a single posting
  - `get_curated_list` — pull a curated list of jobs

## Usage

Point any MCP-compatible client at the endpoint above. No API key, no signup.

```json
{
  "mcpServers": {
    "lokerdollar-jobs": {
      "url": "https://mcp.lokerdollar.com/mcp"
    }
  }
}
```

## About

Built by [LokerDollar](https://lokerdollar.com), a job board for remote roles paying in foreign currency.
