# gg-deploy Announcement

## Twitter/X Thread

```
I got tired of clicking through GoDaddy's UI to set up GitHub Pages. So I built gg-deploy.

One command. Domain + repo → DNS configured, CNAME created, Pages enabled, SSL ready.

It's the tool I wish existed when I was deploying abediaz.ai.

→ https://github.com/abe238/gg-deploy

---

Three ways to use it:

1. CLI: `npx gg-deploy apply example.com user/repo`
2. Web UI: `npx gg-deploy ui` → localhost:3847
3. Claude: Works as an MCP server. Tell Claude "deploy my site" and it just... does.

---

What it actually does:
- Sets A records to GitHub's IPs (185.199.108-111.153)
- Adds www CNAME
- Creates CNAME file in repo
- Enables Pages
- Checks SSL status

Takes 60 seconds. DNS propagation takes longer (that's physics, not me).

---

Built for vibe coders who want their site live NOW.

No clicking through dashboards. No copy-pasting IPs. No remembering which file goes where.

Domain → Repo → Deploy → Done.
```

## LinkedIn Post

```
Just shipped gg-deploy: a CLI for GoDaddy + GitHub Pages deployments.

The problem: Every time I wanted to point a domain at GitHub Pages, I had to:
1. Look up GitHub's IP addresses
2. Add 4 A records in GoDaddy
3. Add a www CNAME
4. Create a CNAME file in my repo
5. Enable Pages in GitHub settings
6. Wait and hope SSL works

Now it's one command: `npx gg-deploy apply example.com user/repo`

Three interfaces:
- CLI for devs
- Local web UI for the click-enjoyers
- MCP server for AI assistants (works with Claude Desktop)

Open source: github.com/abe238/gg-deploy

Built this after deploying abediaz.ai and thinking "I never want to do this manually again."
```

## Hacker News

```
Title: Show HN: gg-deploy – One command to connect GoDaddy domains to GitHub Pages

I kept setting up GitHub Pages for side projects and personal sites. Every time, I'd forget which IPs to use, mess up the CNAME, or miss a step.

gg-deploy automates the whole flow:

    npx gg-deploy apply example.com user/repo

It handles DNS records, repo CNAME file, GitHub Pages config, and SSL verification.

Three interfaces:
- CLI (obvious choice)
- Local web UI for people who prefer clicking
- MCP server for Claude Desktop integration (tell Claude to deploy your site)

Built for my own use case: quickly shipping static sites without context-switching to GoDaddy/GitHub dashboards.

Limitations:
- Only GoDaddy for now (might add Cloudflare later)
- Public repos only unless you have GitHub Pro
- No subdomain support beyond www

Source: https://github.com/abe238/gg-deploy
```

## Key points to emphasize:

1. **Real problem, real solution** - Not theoretical. I used this for abediaz.ai.
2. **Multiple interfaces** - CLI, Web UI, MCP. Pick what works for you.
3. **AI-native** - Works with Claude. That's where things are going.
4. **Honest limitations** - Only GoDaddy. Only www. Only public repos.
5. **Fast shipping** - 60 seconds, not 60 clicks.
