# Cozy Corner — High-Attention Conversion Redesign

A premium redesign of the **Cozy Corner** Shopify storefront (a home & garden / DIY decor
shop), recolored around the marketing/CTA color research on what actually **draws attention
and drives purchases** — not an aesthetic preference. All pink/rose and emerald tones have
been removed.

The redesign is applied to a **draft theme** ("Cozy Corner — Warm Redesign",
`gid://shopify/OnlineStoreTheme/154654212250`) duplicated from the live theme, so the live
store is untouched until the draft is reviewed and published manually in Shopify admin.

## The palette — Attention & Conversion

The research this is built on:
- **Orange** is the most consistently high-converting **CTA / "Add to Cart"** color (action +
  enthusiasm, without red's alarm) — so it's the single "buy" action color sitewide.
- **Red** is the #1 urgency/attention color (impulse, "act now") — reserved for sale badges.
- **High contrast on near-black darks** makes the action color land on the eye first (the
  isolation effect) and reads premium/trustworthy.

| Role | Hex | Where it's used |
|------|-----|-----------------|
| **Orange-red** (the "buy" action) | `#E5471D` | Every button/CTA, sitewide |
| **Urgency red** | `#D81E1E` | Sale badges, high-attention blocks only |
| **Warm off-white** (base bg) | `#FBF8F2` | Page background |
| **Warm neutral** (card tint) | `#F2EDE6` | Card/section backgrounds |
| **Premium near-black** | `#161616` | Dark feature sections, footer, sold-out badge |
| **Secondary dark** | `#2B2A28` | Alternating feature sections |
| **Near-black** (text) | `#1A1A1A` | Body/heading text on light backgrounds |

## Color schemes (theme `config/settings_data.json`)

These are the theme's global schemes, so they cascade to **every page** — home, collections,
collection list, gift card, cart, and customer account.

- **scheme-1** — Off-white bg, near-black text, orange-red CTA (default site scheme)
- **scheme-2** — Warm-neutral cards, orange-red CTA (product/collection cards)
- **scheme-3** — Premium near-black (sold-out badges, dark feature sections, footer), orange-red CTA
- **scheme-4** — Urgency red (sale badges, high-attention blocks)
- **scheme-5** — Secondary dark (alternating feature sections)

## Typography

- Headings: **Cormorant**, Semibold (`cormorant_n6`)
- Body: **Jost** (`jost_n4`)
- Heading scale 115%; subtle button/card shadows (10% opacity) for depth

## Homepage (`templates/index.json`) & Footer (`sections/footer-group.json`)

All hardcoded section colors (formerly emerald/gold/rose) were remapped to the new palette:
emerald → near-black darks, gold/rose accents → orange-red action, soft-rose → warm neutral,
text → near-black.

## A note on Checkout

Shopify **checkout** styling is NOT controlled by these theme files — it lives in the
separate **Checkout & accounts** branding editor (Shopify admin → Settings → Checkout →
Customize). To match the checkout to this palette, set the primary button / accent to
`#E5471D` and the background/text neutrals there. On non-Plus plans, checkout branding
options are limited to what that editor exposes.

## How to go live

1. Open the draft theme **Cozy Corner — Warm Redesign** in the Shopify admin.
2. Use **Preview** to review it across home, collection, cart, gift card, and account pages.
3. Match the **checkout** branding manually (see note above).
4. When happy, click **Publish**.
