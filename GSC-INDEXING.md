# Google Search Console — Indexing Submissions

Track manual URL inspection requests here. Update status when Google confirms indexing.

---

## Submitted

| URL | Submitted | Status |
|-----|-----------|--------|
| https://littlemomentstudio.co.uk/gallery.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/baby-shower-balloons-kent.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/birthday-balloons-kent.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/balloon-garlands-kent.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/the-sky-celebration.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/the-luxe-baby-shower.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/cloud-theme-party-ideas.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/blue-baby-shower-ideas.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/baby-shower-balloon-ideas.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/first-birthday-balloon-ideas.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/teddy-bear-baby-shower-ideas.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/berrylicious-cakes-partner.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/flowers-by-beatrice-kent.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/baby-shower-balloons-ashford.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/baby-shower-balloons-canterbury.html | 18 May 2026 | Pending |
| https://littlemomentstudio.co.uk/faqs.html | 19 May 2026 | Pending |
| https://littlemomentstudio.co.uk/journal.html | 19 May 2026 | Pending |
| https://littlemomentstudio.co.uk/baby-shower-balloons-maidstone.html | 19 May 2026 | Pending |
| https://littlemomentstudio.co.uk/baby-shower-balloons-medway.html | 19 May 2026 | Pending |
| https://littlemomentstudio.co.uk/baby-shower-balloons-tonbridge.html | 19 May 2026 | Pending |

---

## To Submit Next

| URL | Priority |
|-----|----------|
| https://littlemomentstudio.co.uk/baby-shower-balloons-dartford.html | Medium |
| https://littlemomentstudio.co.uk/baby-shower-balloons-gravesend.html | Medium |
| https://littlemomentstudio.co.uk/baby-shower-balloons-rochester.html | Medium |

---

## Already Indexed (no submission needed)

| URL | Confirmed |
|-----|-----------|
| https://littlemomentstudio.co.uk/ | Before 18 May 2026 |
| https://littlemomentstudio.co.uk/baby-shower-balloons-faversham.html | Before 18 May 2026 |
| https://littlemomentstudio.co.uk/baby-shower-balloons-swale.html | Before 18 May 2026 |
| https://littlemomentstudio.co.uk/baby-shower-venues-sittingbourne.html | Before 18 May 2026 |
| https://littlemomentstudio.co.uk/baby-shower-venues-tonbridge.html | Before 18 May 2026 |
| https://littlemomentstudio.co.uk/neutral-baby-shower-ideas.html | Before 18 May 2026 |
| https://littlemomentstudio.co.uk/how-long-do-balloons-last.html | Before 18 May 2026 |

---

## Notes

- Google recommends submitting a handful of URLs per day via URL Inspection
- Status updates can take days to weeks — check back in GSC under Pages > Full report
- Move rows from "To Submit Next" to "Submitted" as you go
- Move rows to "Already Indexed" once GSC confirms

---

## MCP Integration (To Do)

Claude can query GSC directly via an MCP server — index status, impressions, clicks, coverage — instead of updating this file manually.

**Best option:** [AminForou/mcp-gsc](https://github.com/AminForou/mcp-gsc) — 852 stars, actively maintained, simplest setup.

**Setup** — add to Claude Code MCP config (`~/.claude/mcp.json`):
```json
{
  "mcpServers": {
    "gsc": {
      "command": "uvx",
      "args": ["mcp-gsc"],
      "env": {
        "GSC_CREDENTIALS_PATH": "/path/to/credentials.json"
      }
    }
  }
}
```

Requires a Google OAuth credential JSON from Google Cloud Console. Ask Claude to walk through setup when ready.
