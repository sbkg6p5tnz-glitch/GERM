# Cozy Corner — Rose & Emerald Redesign

A premium, attention-grabbing redesign of the **Cozy Corner** Shopify storefront (a home &
garden / DIY decor shop), built to read as a high-end, "Fortune 500" brand rather than a
generic dropshipping store.

The redesign is applied to a **draft theme** ("Cozy Corner — Warm Redesign",
`gid://shopify/OnlineStoreTheme/154654212250`) duplicated from the live theme, so the live
store is untouched until the draft is reviewed and published manually in Shopify admin.

## The palette — Rose & Emerald (luxe)

| Role | Hex | Where it's used |
|------|-----|-----------------|
| **Rose** (CTA/accent) | `#C9748C` | Buttons, primary accents |
| **Soft rose** (card tint) | `#F3DEDC` | Card/section backgrounds |
| **Deep emerald** | `#1F4A38` | Dark feature sections, footer, sold-out badge |
| **Mid emerald** | `#3E7560` | Alternating feature sections |
| **Gold** (sparing accent) | `#C7A062` | Buttons/badges on dark-emerald sections only |
| **Ivory** (base bg) | `#FBF8F2` | Page background |
| **Deep charcoal-emerald** (text) | `#23362C` | Body/heading text |

## Color schemes (theme `config/settings_data.json`)

- **scheme-1** — Ivory background, charcoal-emerald text, rose primary button (default site scheme)
- **scheme-2** — Soft rose cards
- **scheme-3** — Deep emerald (sold-out badges, dark feature sections, footer)
- **scheme-4** — Rose (sale badges, high-attention blocks)
- **scheme-5** — Mid emerald (alternating feature sections)

## Typography

- Headings: **Cormorant**, Semibold (`cormorant_n6`) — an editorial, high-fashion serif
- Body: **Jost** (`jost_n4`) — clean geometric sans that pairs cleanly with Cormorant
- Heading scale bumped to 115% for more presence
- Subtle button/card shadows (10% opacity) added for depth

## Homepage (`templates/index.json`)

- **Best Sellers** — recolored to the palette and repointed from mismatched placeholder
  products (lab equipment, novelty ornaments) to genuinely on-brand home-decor items.
- **Comparison table** — recolored from a hardcoded blue (`#005BD3`/`#334fb4`) to deep/mid
  emerald, with a rose CTA button.
- **Testimonials** — recolored section background/text to the palette; the one card that had
  a hardcoded blue gradient now uses an emerald gradient.
- **Featured product spotlight** — repointed to an on-brand ceramic decor product, badges
  recolored from pink/blue to rose/gold, and all leftover Portuguese dropshipping copy
  rewritten to on-brand English copy.
- **FAQ** — gradient recolored from blue to emerald.
- **Hero banner** — *not yet updated*. The user supplied a finished branded hero graphic
  (headline, subhead, and CTA baked into the image) to replace the current stock photo, but
  getting it onto Shopify's CDN requires either Shopify's staged-upload flow or the
  dedicated image-upload tool — both are blocked by access restrictions in this environment.
  **Next step:** upload the hero image manually via Shopify Admin → Settings → Files, then
  share the resulting file URL/filename so the `image_banner_6pHN7t` section's `image`
  setting can be repointed to it (and the heading/text/button overlay blocks removed, since
  the graphic already contains its own copy).

## Footer (`sections/footer-group.json`)

Recolored from a hardcoded purple (`#624cba`) to deep emerald with a rose newsletter CTA
button, matching the rest of the site.

## How to go live

1. Open the draft theme **Cozy Corner — Warm Redesign** in the Shopify admin.
2. Use **Preview** to review it across home, collection, and product pages.
3. Swap in the hero image (see note above) once it's been uploaded.
4. When happy, click **Publish**.
