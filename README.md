# SEO Starter, a free Claude skill

A free [Claude](https://claude.ai) skill for a fast, foundational on-page SEO check. It looks at the eight things that decide whether a page can rank at all (title, meta, indexability, headings, internal links, alt text, structured data, and the cheap Core Web Vitals wins), then returns a short, prioritised fix list you can act on the same day.

No connector or API key required. It works from the page HTML you can already see.

## Install

Drop the folder into your Claude skills directory:

```
~/.claude/skills/seo-starter/
```

Then invoke it explicitly: run `/seo-starter`, or ask Claude to do a foundational on-page SEO check. It does not auto-activate.

## What is inside

- `SKILL.md`: the skill itself (the eight-check method)
- `references/on-page-checklist.md`: the printable checklist
- `LICENSE.md`: free to use

## What it does, and does not, do

This is the foundation: it finds the obvious on-page wins straight from the HTML. It does not pull live Search Console data, AI-search structure, or the full schema graph. For those, see the deeper skills in the catalog.

## From forgehouse

This skill is a free taste of [forgehouse.ai](https://forgehouse.ai), a curated catalog of proven Claude skills, agents and MCP connectors, built and used on real agency client work and shipped with the proof attached. The deeper SEO skills (live Search Console audits, AI-search structure, full schema markup) live there.

## License

Free to use, no resale. See `LICENSE.md`.
