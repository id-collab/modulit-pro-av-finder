# Connect Modulit Pro AV Finder

Register a remote Streamable HTTP MCP server at https://www.modulit.eu/mcp with no authentication. No repository code needs to run locally and no Modulit, ChatGPT or third-party credentials should be requested for this guest service.

For Cline use type streamableHttp, url https://www.modulit.eu/mcp, disabled false and autoApprove []. For Gemini CLI the root gemini-extension.json declares mcpServers.modulit.httpUrl. The portable plugin uses root plugin.json and mcp.json.

Verify that initialization succeeds and tools/list returns eight tools. A bounded first query is get_products for a public SKU or search_site for an AV task. All results must retain the selected EU/PL storefront and its public-data restrictions.

Do not expose internal account tools or silently enable approval of all tool calls. All customer login, projects, checkout and payments stay outside this guest integration.
