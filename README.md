# MBA Social — landing page

Static site. No build step, no dependencies, no framework.

```
index.html    landing page
terms.html    Terms of Use
privacy.html  Privacy Policy
styles.css    shared stylesheet (all design tokens live in :root)
logo.png      transparent-background logo, generated from logo.jpeg
```

Copy is taken verbatim from the MBA Social website copy deck; only layout and
design are original.

## Run locally

```sh
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy (Vercel)

No configuration needed — import the repo and use the "Other" framework preset
with the repo root as the output directory. Everything is served as-is.

## Before launch — replace these placeholders

Search for `TODO` and `[Your Legal Entity Name]` across the three HTML files.

| Placeholder | Where |
| --- | --- |
| `[Your Legal Entity Name]` | About section + footer of `index.html`, and both legal pages |
| `#TODO-instagram` | header icon, hero CTA, Follow Us |
| `#TODO-threads` | header icon, Follow Us |
| `#TODO-confessions-form` | Confessions CTA (Google Form) |
| `#TODO-btribe` | Placements CTA |

`contact@mbasocial.in` is wired up as a live `mailto:` — make sure the mailbox
exists on the domain.

## Notes

- Instagram and Threads are the only platforms listed anywhere. Do not add
  placeholder icons for platforms that are not in use.
- `MBA Social™` (with the ™) is used in the header and footer; plain
  `MBA Social` in body copy.
- "Established 2019" and "© 2019–2026" must stay consistent across sections.
- The Terms and Privacy pages are bare-bones drafts from the copy deck, not
  legal advice. Have a lawyer review them before launch.
