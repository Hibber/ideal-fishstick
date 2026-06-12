# ideal-fishstick

Home Assistant automation/editing agent setup for GitHub Copilot:

- `ha-mcp` is configured as an MCP server in `.vscode/mcp.json`
- Home Assistant best-practice skills are installed from `homeassistant-ai/skills`

## Configuration

1. Set `HOMEASSISTANT_URL` and `HOMEASSISTANT_TOKEN` when prompted by Copilot.
2. Use the `home-assistant` MCP server in agent mode for:
   - automations/scripts/scenes creation and edits
   - dashboard and YAML updates
   - Home Assistant debugging and diagnostics

## Cloud agent setup

The repository includes `.github/workflows/copilot-setup-steps.yml` to prepare the Copilot cloud agent environment by installing:

- `uv` (for `uvx ha-mcp@latest`)
- Node.js + `skills` package (`npx skills add homeassistant-ai/skills`)
