# Read-only research tools

| Tool | Purpose |
|---|---|
| search_transactions | Search recorded funding and M&A with filters. |
| get_transaction | Retrieve a transaction and its recorded evidence. |
| get_company_history | Follow a company's recorded financing and acquisition history. |
| summarize_activity | Summarize recorded activity, preserving currencies and amount caveats. |
| search_events | Find legal/legaltech event candidates. |
| get_event | Retrieve event details, sources and uncertainty. |

Exact argument schemas are exposed through MCP tool discovery. No write/admin tool is provided. Query text searches company, buyer, investor, product and category text; use the transaction type filter for funding-only results rather than adding the word “funding” as a generic keyword. Date basis and review filters affect results. Preserve pending/reviewed distinctions, announcement/completion milestones, extensions and unconvertible currencies in answers.
