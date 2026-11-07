<p align="center"><img src="./modulit.png" alt="Modulit" width="96" height="96"></p>

# Modulit Pro AV Finder

The official guest MCP connection for Modulit EU and Poland, published by **UAB Modulit Solutions**, Lithuania.

Find professional audiovisual equipment and published installation solutions by task, model, SKU, signal format or cable distance. Compare alternatives, calculate cable runs, and configure supported AV hardware using Modulit's native calculation logic.

## Connect

- **MCP endpoint:** `https://www.modulit.eu/mcp`
- **Transport:** Streamable HTTP
- **Authentication:** none. No account or API key is needed.
- **Connection guide:** https://www.modulit.eu/mcp-guide/
- **Official MCP Registry:** `eu.modulit/pro-av-finder`
- **Registry record:** https://registry.modelcontextprotocol.io/v0.1/servers/eu.modulit%2Fpro-av-finder/versions/1.0.0
- **Verified Glama listing:** https://glama.ai/mcp/connectors/eu.modulit/pro-av-finder

Choose a remote MCP connection in your client and enter the endpoint. The server supports both EU and Polish storefronts. Storefront visibility and geographic restrictions apply.

### Cursor

Add this entry to your MCP settings:

```json
{"mcpServers":{"modulit":{"url":"https://www.modulit.eu/mcp"}}}
```

The root `plugin.json` and `mcp.json` also provide a portable Agent Plugins package.

### VS Code

In `.vscode/mcp.json` use:

```json
{"servers":{"modulit":{"type":"http","url":"https://www.modulit.eu/mcp"}}}
```

### Cline

Use MCP Servers > Remote Servers, enter the endpoint and select **Streamable HTTP**. For manual configuration:

```json
{"mcpServers":{"modulit":{"type":"streamableHttp","url":"https://www.modulit.eu/mcp","disabled":false,"autoApprove":[]}}}
```

### Gemini CLI

This repository includes `gemini-extension.json` with a direct HTTP connection:

```sh
gemini extensions install https://github.com/id-collab/modulit-pro-av-finder
```

### ChatGPT and other MCP clients

Follow the client-specific instructions in the [Modulit connection guide](https://www.modulit.eu/mcp-guide/). ChatGPT public-directory review is pending; use its custom-MCP workflow where your plan supports it. Login to ChatGPT does not grant access to a Modulit customer account.

## What you can do

| Tool | Purpose |
|---|---|
| `search_site` | Find published Modulit solutions, guides, equipment and tools by task or model. |
| `search_products` | Search the catalogue with technical constraints. |
| `get_products` | Look up up to 20 exact products and public commercial information. |
| `search_product_analogs` | Find alternatives while retaining technical requirements. |
| `calculate_cable_route` | Calculate cable lengths using native site logic. |
| `describe_power_selector` | Discover supported power-selector parameters. |
| `configure_power` | Run the supported native power configuration. |
| `configure_mediahub` | Produce a supported Mediahub configuration and parts list. |

## Try these requests

- Find two HDMI cables for 4K60 over 40 metres on Modulit PL. Link the matching models and distinguish confirmed specifications from unknowns.
- Find a published Modulit EU guide about extending a USB camera and microphone in a meeting room.
- Calculate three direct 40 metre cable runs, with no loops, height changes or waste allowance.
- Configure three PureLink Mediahub ENC10 sets using preset 1 on Modulit PL. Show quantities per set and totals.
- Look up 1T-C2-100 on Modulit EU and show the price and availability visible to a guest.

## Public commercial information

Suggested retail prices, when public on the selected storefront, are labelled MSRP with their currency and VAT basis. Some brands require a Modulit login and expose no guest price. Availability is only the public storefront label, never an inferred exact warehouse count. An unconfirmed value stays unknown.

This guest service is read-only. It does not expose personal prices, exact warehouse quantities, customer projects, reservations, orders or payments. Product availability checks do not reserve stock.

## Privacy and support

- [Privacy and cookies](https://www.modulit.eu/privacy-and-cookie-policy/)
- [Terms](https://www.modulit.eu/terms-of-sale/)
- [Company and support](https://www.modulit.eu/contacts-en/)
- Technical contact: id@modulit.eu

This repository contains public connection metadata and client documentation for the hosted service. The hosted service is operated by UAB Modulit Solutions. Modulit names and logos remain their owners' trademarks.
