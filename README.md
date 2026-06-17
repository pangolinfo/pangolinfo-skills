# Pangolinfo Skills

Amazon e-commerce AI agent skills, powered by the [Pangolinfo MCP server](https://github.com/pangolinfo/pangolinfo-mcp).

Each skill is a self-contained `SKILL.md` that teaches an AI agent (Claude Code, Cursor, Cline, Windsurf, Codex, and other MCP-capable clients) a complete Amazon research workflow — when to trigger it, which Pangolinfo MCP tools to chain, and how to turn raw data into a usable answer.

## Quick install — copy this to your AI assistant

Don't unzip anything yourself. Just paste the block below to the AI agent you already use (Claude Code, Cursor, Cline, …) and it will install all 6 skills into the right place for your client.

> **English**
>
> Please install the Pangolinfo Amazon skills for me:
> 1. Download this bundle: `https://github.com/pangolinfo/pangolinfo-skills/archive/refs/heads/main.zip`
> 2. Unzip it — inside `pangolinfo-skills-main/` there are 6 skill folders (`amazon-product-explorer`, `pangolinfo-amazon-niche`, `pangolinfo-amazon-scraper`, `amazon-daily-competitor-radar`, `amazon-listing-optimization`, `pangolinfo-ai-serp`), each containing a `SKILL.md`.
> 3. Copy those 6 skill folders into the skills directory that YOUR client loads skills from (for Claude Code that's `~/.claude/skills/`). Skip `README.md`, `LICENSE`, and `.gitignore`.
> 4. These skills call the Pangolinfo MCP server — confirm it's connected and that I have a Pangolinfo API key (get one at https://www.pangolinfo.com).
> 5. When done, list the 6 skills you installed so I can confirm.

> **中文**
>
> 请帮我安装 Pangolinfo 亚马逊 skills：
> 1. 下载这个压缩包：`https://github.com/pangolinfo/pangolinfo-skills/archive/refs/heads/main.zip`
> 2. 解压 —— `pangolinfo-skills-main/` 里有 6 个 skill 文件夹（`amazon-product-explorer`、`pangolinfo-amazon-niche`、`pangolinfo-amazon-scraper`、`amazon-daily-competitor-radar`、`amazon-listing-optimization`、`pangolinfo-ai-serp`），每个里面有一个 `SKILL.md`。
> 3. 把这 6 个 skill 文件夹复制到**你所在客户端**加载 skills 的目录（Claude Code 是 `~/.claude/skills/`）。跳过 `README.md`、`LICENSE`、`.gitignore`。
> 4. 这些 skill 依赖 Pangolinfo MCP 服务 —— 确认它已连接、且我有 Pangolinfo API key（到 https://www.pangolinfo.com 获取）。
> 5. 装完后列出你安装的 6 个 skill 让我确认。

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
