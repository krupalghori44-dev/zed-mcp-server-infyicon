# Infyicon Free Icons — Zed extension

Gives Zed's agent an MCP context server for [Infyicon](https://infyicon.com): **161,000+ free hand-drawn vector icons** in four matching styles (outline, fill, color-outline, color-fill), with ready-to-embed SVG markup and transparent PNG URLs. No account, no API key.

## Install

Zed → Extensions → search **Infyicon** → Install. The extension pulls the `infyicon-mcp` npm package (a zero-dependency relay to the hosted server at `https://infyicon.com/mcp`) and runs it with Zed's bundled Node.js. Nothing to configure.

Then, in the agent panel: *"find a shopping cart icon and give me the SVG"*.

## Tools

| Tool | What it does |
|---|---|
| `search_icons` | Keyword search with optional style filter and paging |
| `get_popular_icons` | Featured icons when there is no search term |
| `get_related_icons` | Same-theme icons across styles |
| `get_icon_svg` / `get_icon_svg_bulk` | Ready-to-embed SVG markup (1 or 1–20 ids) |
| `get_icon_png` | Transparent PNG URLs at 16–512 px |
| `list_categories` | Popular categories with counts |
| `search_uicons` | CSS class names in the Infyicon UI webfont |

Manual alternative (no extension): add to `settings.json`

```json
{ "context_servers": { "infyicon": { "command": { "path": "npx", "args": ["-y", "infyicon-mcp"] } } } }
```

## License

Extension: MIT. Icons: free with attribution to infyicon.com — https://infyicon.com/license. Server source: https://github.com/krupalghori44-dev/infyicon-mcp · all clients: https://infyicon.com/connect