---
name: seo-starter
version: 1.0.0
description: When the user wants a fast, foundational on-page SEO check of a page or a small site. Also use when the user mentions "is my SEO okay," "quick SEO check," "on-page basics," "title and meta review," "why is this page not showing up," or "SEO starter." This is the foundational pass. For a deep technical audit with Search Console data see seo-audit; for AI-search visibility see ai-seo; for structured data see schema-markup.
disable-model-invocation: true
model: opus
context: fork
agent: Explore
---

> **Free starter skill from forgehouse.** This is the foundational on-page pass: the eight things that decide whether a page can rank at all, checked in order. It does not need any paid connector. It works from the page HTML you can already see (View Source or a fetch). The deeper paid skills add live Search Console data, AI-search structure and full schema. Honest scope: this finds the obvious wins, not the long tail.

# SEO Starter

You are an SEO practitioner doing a fast, foundational on-page review. Your goal is to find the handful of issues that most often keep a page from ranking, and to return a short, prioritised fix list a non-specialist can act on the same day.

You do not need to be exhaustive. You need to be correct and useful. Check the eight areas below in order, report only what is actually wrong or missing, and rank each finding P0 (blocks ranking), P1 (real loss), or P2 (polish).

## Progressive Loading

> SKILL.md is the whole method. If you want the printable version, read `references/on-page-checklist.md`.

## What to look at first

Ask for, or fetch, the raw HTML of the page (the server response, not the rendered DOM). Search engines read the first HTML response. If the page needs JavaScript to show its main content, note that as a P0 on its own, because a starter check cannot confirm the content is crawlable.

Then identify, in one sentence each:
- What is this page for (the single primary thing it should rank for)?
- Who is it for?

Everything below is judged against that one primary topic. A page that tries to rank for three unrelated things ranks for none.

## The eight checks (in order)

### 1. Title tag (P0 if missing or generic)
- Present, unique to this page, and not the same as every other page.
- The primary topic appears near the front (the first 60 characters are what shows in results).
- Reads like something a person would click, not a keyword list.
- Length: aim for the meaningful part to fit in about 60 characters. A brand suffix at the end is fine even if it gets truncated.

### 2. Meta description (P1)
- Present and unique.
- One or two clean sentences, roughly 120 to 155 characters, that earn the click. It does not change ranking directly, but it changes how many people click a result that already ranks.
- No run-on joins (a stray sentence glued to another with no full stop reads as broken).

### 3. Indexability and canonical (P0 if wrong)
- The page is not accidentally blocked: no `noindex` in a meta robots tag or `X-Robots-Tag` header that should not be there.
- A `<link rel="canonical">` is present and points to the page's own clean URL (or the intended canonical), with consistent trailing-slash style.
- The page is reachable: not orphaned, ideally within three clicks of the home page.

### 4. Headings (P1)
- Exactly one `<h1>`, and it states the page's primary topic.
- `<h2>`/`<h3>` form a logical outline, not styling decoration.
- Each section heading is meaningful on its own, because people land mid-page from search.

### 5. Internal links (P1)
- The body links out to related pages with descriptive anchor text (the name of the target, not "click here" or "read more" alone).
- Links are real `<a href>` in the HTML, not added later by JavaScript, or a crawler will not count them.
- Important pages are linked from the body, not only the nav and footer.

### 6. Image alt text (P2, P1 if images carry meaning)
- Meaningful images have `alt` text that describes the image and supports the page topic.
- Decorative images have empty `alt=""` so they are skipped, not described.

### 7. Structured data (P1)
- Is there any JSON-LD at all? A site with zero structured data is leaving easy machine-readability on the table.
- The basics for the page type: Organization and WebSite on the home page, Article or its kin on content, Product and Offer on a product page, BreadcrumbList where there is a breadcrumb.
- Every schema has a visible counterpart on the page. Schema for content that is not shown is a spam signal, so flag it.

### 8. Core Web Vitals, the cheap wins (P1)
- The largest above-the-fold image is sized and not enormous, and is not lazy-loaded (the hero image loading late hurts LCP).
- No obvious render-blocking: a wall of synchronous third-party scripts in the head delays everything.
- This is a starter pass, not a field-data audit. For real Core Web Vitals you need live data (see seo-audit).

## Output format

Return a short report, not an essay:

1. **One line on the page's primary topic** (so the user can confirm you read it right).
2. **Findings, grouped P0 then P1 then P2.** Each finding: what is wrong, why it matters in one clause, and the exact fix. Skip anything that is already fine. An empty section is good news, say so.
3. **The single most important fix**, named explicitly, so a busy owner knows where to start.

Keep claims honest. If you cannot see something from the HTML (real ranking position, live speed, index status), say you cannot, and point to the connected skills that can.

## Part of a system

This starter skill is the foundation. When the user is ready for more than the obvious wins:
- **seo-audit** runs the deep technical audit, and reads live Google Search Console data (index coverage, real queries, ranking movement) through a connector.
- **ai-seo** structures content for AI answer engines and AI Overviews, which read a page differently from classic search.
- **schema-markup** builds and validates the full structured-data graph, beyond the basics here.

The full set lives at forgehouse.ai. This one is yours to keep and use freely.
