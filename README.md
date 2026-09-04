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

## Outbound links

All live — no placeholders remain.

| Destination | Where it appears |
| --- | --- |
| `https://instagram.com/mbasocial` | header icon, hero CTA, Follow Us |
| `https://www.threads.com/@mbasocial` | header icon, Follow Us |
| `https://forms.gle/BZrCALY5LaeDaChQ8` | Confessions CTA |
| `https://www.btribe.in` | Placements CTA |
| `contact@mbasocial.in` | Contact section, both legal pages |

`contact@mbasocial.in` is wired up as a live `mailto:` — make sure the mailbox
exists on the domain before launch.

Canonical URLs and Open Graph tags assume the site is served from
`https://mbasocial.in/`.

## Notes

- Instagram and Threads are the only platforms listed anywhere. Do not add
  placeholder icons for platforms that are not in use.
- `MBA Social™` (with the ™) is used in the header and footer; plain
  `MBA Social` in body copy.
- "Established 2019" and "© 2019–2026" must stay consistent across sections.
- There is no registered legal entity, so the copy reads "independently owned
  and operated" and the footer is just the copyright line. If an entity is
  registered later, name it in the About section, the footer, and both legal
  pages — consistently, in the exact registered form.
- The Terms and Privacy pages are bare-bones drafts from the copy deck, not
  legal advice. Have a lawyer review them before launch.
