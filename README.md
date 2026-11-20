# UpInvoice

[UpInvoice](https://upinvoice.eu) reads supplier invoices, purchase orders and customer orders (PDF, scan or phone photo) with its own extraction AI and returns structured data: supplier or customer, references, dates, totals, VAT and product lines, checked against the document totals. It can create the documents directly in Dolibarr ERP.

## Build with UpInvoice

| | |
|---|---|
| **REST API** | One endpoint for invoices and orders, idempotent retries, OpenAPI 3.1 spec. [Developer docs](https://upinvoice.eu/developers) · [openapi.yaml](https://upinvoice.eu/openapi.yaml) |
| **Agent skill** | Lets Claude Code, Claude.ai, Cursor and other agents integrate the API for you. [upinvoice/skills](https://github.com/upinvoice/skills) |
| **MCP server** | Connect Claude, Cursor, VS Code and other assistants to `https://upinvoice.eu/mcp` and extract documents without writing code. [Setup](https://upinvoice.eu/developers/mcp) |
| **Dolibarr module** | Free module (GPL v3) that sends your documents to UpInvoice and creates the result in Dolibarr. [upinvoice/module_upinvoice](https://github.com/upinvoice/module_upinvoice) |

Install the skill in Claude Code:

```bash
claude plugin marketplace add upinvoice/skills
claude plugin install upinvoice-api@upinvoice
```

## Pricing

Each processed document costs one credit. Credits come with a monthly or yearly plan, or as extra credit packs, and every new account gets 10 free documents. See [upinvoice.eu/prices](https://upinvoice.eu/prices).

## Contact

[upinvoice.eu](https://upinvoice.eu) · info@upinvoice.eu
