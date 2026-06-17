# Pangolinfo Skills

Amazon e-commerce AI agent skills, powered by the [Pangolinfo MCP server](https://github.com/pangolinfo/pangolinfo-mcp).

Each skill is a self-contained `SKILL.md` that teaches an AI agent (Claude Code, Cursor, Cline, Windsurf, Codex, and other MCP-capable clients) a complete Amazon research workflow — when to trigger it, which Pangolinfo MCP tools to chain, and how to turn raw data into a usable answer.

## Skills

| Skill | What it does |
|---|---|
| [`amazon-product-explorer`](amazon-product-explorer/SKILL.md) | 从 0 到 1 选品 / 蓝海利基挖掘。"what should I sell" / "find a blue-ocean niche" / "新品立项"。 |
| [`pangolinfo-amazon-niche`](pangolinfo-amazon-niche/SKILL.md) | 类目树浏览 + 按销量/搜索量/退货率/竞争度筛利基。"browse Amazon category tree" / "find low-competition niches"。 |
| [`pangolinfo-amazon-scraper`](pangolinfo-amazon-scraper/SKILL.md) | 抓商品/ASIN 详情、搜索列表、榜单、批量评论 VOC。"scrape this ASIN" / "get reviews for B0XXX"。 |
| [`amazon-daily-competitor-radar`](amazon-daily-competitor-radar/SKILL.md) | 每日竞品监控:价格、排名、Buy Box 变化。"track ASIN X" / "daily radar"。 |
| [`amazon-listing-optimization`](amazon-listing-optimization/SKILL.md) | Listing 文案优化:标题、五点、Search Terms、VOC 分析。"rewrite my listing"。 |
| [`pangolinfo-ai-serp`](pangolinfo-ai-serp/SKILL.md) | Google 站外需求/舆情调研:SERP、AI Overview、引文来源、趋势对比。"search Google for X"。 |

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
