# Cozy Corner — Warm Redesign

A color + styling redesign of the **Cozy Corner** Shopify storefront (a home & garden / DIY decor shop).
The goal: a 3-color palette grounded in color-psychology research that grabs attention while still
reading as elegant, warm, and homey.

The redesign is applied to a **draft theme** ("Cozy Corner — Warm Redesign") duplicated from the live
theme, so the live store is untouched until the draft is reviewed and published.

## The palette

| Role | Hex | Where it's used | Why |
|------|-----|-----------------|-----|
| **Terracotta** (accent / CTA) | `#C2643F` | Buttons, "Add to cart", sale badges | Warm orange-reds are the strongest attention + urgency drivers; CTA color changes in this family have lifted click-through 20–30%+. |
| **Sage green** (supporting) | `#6E7E5C` / deep `#4F5D45` | Feature sections, sold-out badges | Green signals nature / garden, calm, and trust; green-leaning schemes convert well for general retail. |
| **Warm cream** (base) | `#FAF5EC` | Page backgrounds | Warm neutrals read as cozy, homey, and elegant — the preferred décor palette. |
| Espresso (text) | `#3D332A` | Body + heading text | Soft warm dark instead of harsh black, for an elegant feel and strong contrast. |
| Sand (cards) | `#EFE6D6` | Product / collection cards | Subtle warm separation from the cream background. |

Color drives up to ~90% of snap product judgments and shoppers form a first impression in ~50ms, so a
cohesive warm-plus-accent scheme is doing real conversion work, not just decoration.

## Color schemes (theme `config/settings_data.json`)

- **scheme-1** — Cream background, espresso text, terracotta primary button (the default site scheme)
- **scheme-2** — Sand cards
- **scheme-3** — Deep sage (sold-out badges, dark feature sections)
- **scheme-4** — Terracotta (sale badges, high-attention blocks)
- **scheme-5** — Mid sage (alternating feature sections)

## Other styling changes

- Headings set to an elegant serif (**Playfair Display**) over a clean body font (**Assistant**)
- Heading scale bumped to 110% for presence
- Softer, rounder buttons / cards / inputs / media (8–12px radius), thinner 1px borders
- Subtle hover animations enabled

## How to go live

1. Open the draft theme **Cozy Corner — Warm Redesign** in the Shopify admin.
2. Use **Preview** to review it across home, collection, and product pages.
3. When happy, click **Publish**.

> Sources informing the palette: color-psychology / ecommerce-conversion research
> (alidropship, attentioninsight, dragonflyai, productiveshop, coschedule, and others).
