# On-page SEO starter checklist

The printable version of the eight checks. Go in order. Mark each P0, P1, P2, or OK. Stop guessing and look at the raw HTML response, not the rendered page.

## Before you start
- [ ] One sentence: what is this page meant to rank for?
- [ ] One sentence: who is it for?
- [ ] Is the main content in the first HTML response, or does it need JavaScript? (JS-only main content = P0)

## 1. Title tag
- [ ] Present and unique to this page
- [ ] Primary topic in the first ~60 characters
- [ ] Reads like a click, not a keyword list

## 2. Meta description
- [ ] Present and unique
- [ ] ~120 to 155 characters, one or two clean sentences
- [ ] No run-on (no sentence glued to another without a full stop)

## 3. Indexability and canonical
- [ ] No accidental `noindex` (meta robots or `X-Robots-Tag`)
- [ ] `rel="canonical"` present, points to the right clean URL
- [ ] Trailing-slash style is consistent
- [ ] Page is within ~3 clicks of the home page

## 4. Headings
- [ ] Exactly one `<h1>`, stating the primary topic
- [ ] `<h2>`/`<h3>` form a logical outline
- [ ] Each section heading makes sense on its own

## 5. Internal links
- [ ] Body links use descriptive anchor text (the target's name)
- [ ] Links are real `<a href>` in the HTML, not JS-injected
- [ ] Important pages linked from the body, not only nav and footer

## 6. Image alt text
- [ ] Meaningful images have descriptive `alt`
- [ ] Decorative images have empty `alt=""`

## 7. Structured data
- [ ] Some JSON-LD exists
- [ ] The basics for the page type are present (Organization/WebSite on home, Article on content, Product/Offer on product, BreadcrumbList where shown)
- [ ] Every schema has a visible counterpart on the page

## 8. Core Web Vitals, cheap wins
- [ ] Hero image is sized sensibly and not lazy-loaded
- [ ] No wall of synchronous third-party scripts in the head
- [ ] (Real field data needs a connector. This is a starter pass.)

## Report
- [ ] One line confirming the page's primary topic
- [ ] Findings grouped P0, then P1, then P2, each with the exact fix
- [ ] The single most important fix, named
- [ ] Honest about anything the HTML alone cannot show
