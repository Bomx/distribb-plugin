# SEO with Distribb

The official [Distribb](https://distribb.io) plugin. It turns your coding agent into a working SEO operator: keyword research, articles that earn real high-DR backlinks, publishing straight into your CMS, internal linking, and Google Business Profile management.

Built to the [Agent Plugins](https://agent-plugins.org) 1.0.0 standard, so it loads in Cursor and any other conformant client without changes.

## What you get

**A skill** that teaches the agent the actual SEO process, in order: connect your site and Search Console, audit first, build topic clusters, then research keywords, write, earn links, and optimize. It ships 18 slash commands, an audit playbook, and a 90-day sprint sub-skill.

**An MCP server** at `https://distribb.io/mcp` with 18 tools:

| Area | Tools |
| --- | --- |
| Projects | `list_projects`, `get_project`, `create_project`, `update_project` |
| Articles | `list_articles`, `get_article`, `create_article`, `update_article`, `publish_article` |
| Research | `keyword_research`, `search_console_performance`, `ai_visibility_report` |
| Backlinks | `backlinks_status`, `list_backlinks` |
| Google Business Profile | `gbp_status`, `gbp_reviews`, `gbp_reply_review` |
| Setup | `list_integrations` |

Eleven are read-only. The seven that write are annotated so your client knows which ones touch the outside world: `publish_article`, `update_article` and `gbp_reply_review` can change something the public can see, and prompt before they do.

## Install

In Cursor, open **Customize**, find **Distribb** in the Marketplace, and install.

To install from source, point your client at this repository. The plugin root holds `plugin.json` and `mcp.json`; the skill lives in `skills/distribb/`.

## Connecting your account

The MCP server uses OAuth 2.0 with PKCE. Your client opens a Distribb consent page, you approve, and it stores the token. No API key to copy, and no credentials live in this repository.

You need a [Distribb account](https://distribb.io). Keyword research and the SEO audit work on every plan. Article generation requires a paid plan.

## Support

[distribb.io](https://distribb.io) | support@distribb.io

## License

MIT. See [LICENSE](LICENSE).
