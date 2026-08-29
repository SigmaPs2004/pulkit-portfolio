# Pulkit Soni — Product Portfolio

Single-page static portfolio. No build step, no dependencies.

```
index.html   # the whole site (nav, hero, experience, case studies, teardowns, decks, about, contact)
style.css    # design system: warm slate + teal palette, all values as CSS variables
images/      # logos, deck covers, profile photo
```

## Design system

| Token | Value | Use |
| --- | --- | --- |
| `--ink` | `#1C2321` | headings, contact band, footer |
| `--slate` | `#2E3A38` | body text |
| `--cream` | `#F6F4EF` | page background |
| `--teal` | `#1E8E7E` | CTAs, links, active nav, card hover |

Type: Fraunces (headings) + Inter (body), loaded from Google Fonts.

## Notes

- Every card (case study, teardown, deck) is a single `<a>` wrapping the whole tile, so the entire card is clickable — not just the text.
- Section order is deliberate: proof of work (experience → case studies → teardowns → decks) comes before the personal story and contact.
- Nav is sticky with the in-view section highlighted; horizontally scrollable on mobile.
- Update copy or links directly in `index.html`.

## Publishing to GitHub Pages

Push these files to the repository root (or a `docs/` folder) and enable Pages for that branch/folder. Update the `canonical` and `og:*` URLs in `index.html` to your live domain.
