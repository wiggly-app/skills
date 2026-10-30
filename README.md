# Wiggly Agent Skills

Official agent skills for [Wiggly](https://wiggly.agentenamel.com).

Skills teach your AI agents (Claude, Cursor, Codex, ChatGPT, Antigravity) how to direct, author, and produce on-brand videos and animations powered by the Wiggly Studio MCP server.

---

## Quick Install

Add any skill to your agent with the `skills` CLI:

```bash
# My Pixar Story — 3D Animated Family Memoir
npx skills add wiggly-app/skills -s my-pixar-story
```

---

## MCP Server Connection

All Wiggly creative formats render via the hosted Wiggly MCP server:

- **Endpoint**: `https://wiggly.agentenamel.com/mcp`
- **Transport**: HTTP / SSE

### Claude Code
```bash
claude mcp add --transport http wiggly https://wiggly.agentenamel.com/mcp
```

### Cursor / VS Code
Add to `.cursor/mcp.json` or `.vscode/mcp.json`:
```json
{
  "mcpServers": {
    "wiggly": {
      "url": "https://wiggly.agentenamel.com/mcp"
    }
  }
}
```

### Claude Desktop
Add to your Claude Desktop configuration:
```json
{
  "mcpServers": {
    "wiggly": {
      "url": "https://wiggly.agentenamel.com/mcp"
    }
  }
}
```

---

## Available Skills

| Skill | Description | Install Command |
|---|---|---|
| **My Pixar Story** | Turn family questionnaire memories into a cinematic 3D animated memoir (Pixar-style) | `npx skills add wiggly-app/skills -s my-pixar-story` |

---

## License

MIT © [Wiggly](https://wiggly.agentenamel.com)
