# Pangolinfo Skills

Amazon e-commerce AI agent skills, powered by the [Pangolinfo MCP server](https://github.com/pangolinfo/pangolinfo-mcp).

Each skill is a self-contained `SKILL.md` that teaches an AI agent (Claude Code, Cursor, Cline, Windsurf, Codex, and other MCP-capable clients) a complete Amazon research workflow — when to trigger it, which Pangolinfo MCP tools to chain, and how to turn raw data into a usable answer.

## Skills

| Skill | What it does |
|---|---|
| [`amazon-product-explorer`](amazon-product-explorer/SKILL.md) | Product discovery & blue-ocean niche scouting from scratch. Triggers: "what should I sell", "find a blue-ocean niche", "is X category worth entering", "launch a new product". |
| [`pangolinfo-amazon-niche`](pangolinfo-amazon-niche/SKILL.md) | Browse the Amazon category tree and filter niches by sales / search volume / return rate / competition. Triggers: "browse Amazon category tree", "find low-competition niches", "filter categories by metrics". |
| [`pangolinfo-amazon-scraper`](pangolinfo-amazon-scraper/SKILL.md) | Scrape product/ASIN details, search listings, bestseller & new-release rankings, and bulk reviews for VOC. Triggers: "scrape this ASIN", "get reviews for B0XXX", "category bestsellers". |
| [`amazon-daily-competitor-radar`](amazon-daily-competitor-radar/SKILL.md) | Daily competitor monitoring — price, rank, and Buy Box changes. Triggers: "track ASIN X", "daily radar", "did my ranking drop", "did I lose the Buy Box". |
| [`amazon-listing-optimization`](amazon-listing-optimization/SKILL.md) | Listing copy optimization — title, bullets, Search Terms, and VOC analysis. Triggers: "rewrite my listing", "improve my title", "my conversion is low". |
| [`pangolinfo-ai-serp`](pangolinfo-ai-serp/SKILL.md) | Off-Amazon demand & sentiment research via Google — SERP, AI Overview, citation sources, trend comparison. Triggers: "search Google for X", "what does AI Overview say", "compare A vs B trends". |

## Prerequisites

These skills call the Pangolinfo MCP server's tools. You need:

1. The **Pangolinfo MCP server** connected to your AI client — see [pangolinfo-mcp](https://github.com/pangolinfo/pangolinfo-mcp).
2. A **Pangolinfo API key** — get one at <https://www.pangolinfo.com> (new users receive free credits).

## Install

Copy the skill folders into your AI client's skills directory. For Claude Code:

```bash
git clone https://github.com/pangolinfo/pangolinfo-skills.git
mkdir -p ~/.claude/skills/pangolinfo
cp -r pangolinfo-skills/*/ ~/.claude/skills/pangolinfo/
```

Other clients use different skill paths — place each skill folder wherever your client loads skills from.

## License

[MIT](LICENSE) © 2026 Pangolinfo
