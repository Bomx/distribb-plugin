# SEO with Distribb

The official [Distribb](https://distribb.io) plugin. It turns your coding agent into a working SEO operator: keyword research, articles that earn real high-DR backlinks, publishing straight into your CMS, internal linking, Google Business Profile management, social publishing, paid ads, and every other integration you connect on Distribb.

Built to the [Agent Plugins](https://agent-plugins.org) 1.0.0 standard, so it loads in Cursor and any other conformant client without changes.

## What you get

**A skill** that teaches the agent the actual SEO process, in order: connect your site and Search Console, audit first, build topic clusters, then research keywords, write, earn links, and optimize. It ships 20 slash commands, playbooks for SEO, social media, outreach, paid ads and integrations, an audit playbook, and a 90-day sprint sub-skill.

**An MCP server** at `https://distribb.io/mcp` with 40 tools:

| Area | Tools |
| --- | --- |
| Projects | `list_projects`, `get_project`, `create_project`, `update_project`, `start_onboarding`, `set_article_plan` |
| Articles | `list_articles`, `get_article`, `get_article_brief`, `create_article`, `update_article`, `publish_article`, `upload_image`, `screenshot_page` |
| Research | `keyword_research`, `search_console_performance`, `ai_visibility_report` |
| Optimizations | `list_optimizations`, `get_optimization`, `review_optimization`, `publish_optimization` |
| Backlinks | `backlinks_status`, `list_backlinks` |
| Social | `list_social_accounts`, `upload_social_media`, `publish_social_post`, `get_social_post`, `list_social_posts`, `configure_social_post_auto_reply` |
| Google Business Profile | `gbp_status`, `gbp_reviews`, `gbp_reply_review` |
| Every integration | `list_integrations`, `integrations_catalog`, `connect_integration`, `find_integration_tools`, `run_integration_read`, `run_integration_action`, `get_integration_result` |
| Playbooks | `get_playbook` (SEO, social media, outreach, paid ads, integrations) |

The integration tools reach everything you connect on Distribb: ad accounts (Meta, Google, TikTok, LinkedIn), social inboxes, DMs and comments, analytics tools, bank accounts, outreach and email tools, databases, GitHub, and new integrations as Distribb adds them, with the same permissions and preview-then-confirm rule as Distribb's own agent. Connecting stays with you: the agent sends a link that opens the right card on Distribb.

23 tools are read-only. The 17 that write are annotated so your client knows which ones touch the outside world, and the ones that can change something the public sees (publishing, review replies, social posts, integration actions such as launching a campaign) prompt before they run.

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
