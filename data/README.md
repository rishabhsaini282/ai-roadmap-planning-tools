# data/ — Column Definitions & Source Notes

## File: `ai-pm-tools-data.csv`

20 AI PM tools across 6 workflow categories, compiled from in-depth analysis published June 2026. Each row is independently verifiable.

### Column Definitions

| Column | Description |
|---|---|
| `tool_name` | Official product name as of June 2026 |
| `category` | Primary PM workflow the tool addresses (Roadmap Planning, PRD Writing, User Research, Prototyping, General AI Assistant, Collaboration) |
| `core_ai_feature` | The specific AI capability that differentiates this tool from a non-AI alternative |
| `free_tier` | Whether a free tier exists (Yes/No) |
| `free_tier_limit` | Specific constraint where the free tier breaks down for real PM usage |
| `paid_price_usd_per_user_per_month` | Base paid tier price in USD per user per month as of June 2026 — "Contact sales" means no public pricing |
| `pricing_model` | Per-seat, usage-based, credit-based, or bundled |
| `jira_sync` | Whether native bi-directional Jira sync exists (Bi-directional / One-way / Via integration / No / Native) |
| `best_workflow` | The single PM workflow where this tool has the clearest ROI |
| `notable_limitation` | The most common reason a team drops or avoids this tool |
| `source_article` | Full URL to the source article where this data was verified |

### Notes on Pricing

- Prices reflect publicly listed rates as of June 2026
- "Bundled" means the AI feature is included in an existing paid plan without a separate line item
- Enterprise pricing (contact sales) typically starts at 5–10x the listed per-seat rate
- Prices are in USD; purchasing power parity applies — Indian market prices may differ by 20–40%

### Known Data Gaps

- UserTesting and EnjoyHQ do not publish pricing; figures marked "Contact sales" are accurate as of June 2026 but may change
- Token/credit burn rates for usage-based tools (v0, Bolt, Lovable) vary by prompt complexity and are not listed as they cannot be meaningfully compared on a per-user basis

### Sources

All data compiled from the following articles on Product Leaders Day India:

- https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/ai-tools-for-product-managers.html
- https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/ai-roadmap-planning-tools.html
- https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/ai-prd-writing-tools.html
- https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/ai-user-research-tools.html
- https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/ai-prototyping-tools-for-pms.html
- https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/free-ai-tools-for-product-managers.html
- https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/ai-pm-tools-pricing-compared.html
