---
name: magic-item-pricing
description: Roll the cost of a magic item by rarity using the owner's house rule. Use when generating a magic item and it needs a value.
---

# Magic item pricing

The owner's house rule for the cost of a magic item, by rarity. It applies to all of the owner's games, in every world in this repo. It is not a published rule.

## Cost by rarity

| Rarity | Cost |
|--------|------|
| Common | 3d100 gp |
| Uncommon | 1d100 pp |
| Rare | 5d100 pp |
| Very Rare | 1d100 pp × 10 |

- `pp` is platinum pieces. 1 pp is 10 gp.
- For Very Rare, the 1d100 roll is multiplied by 10.
- There is no Legendary tier. If a Legendary item comes up, ask the owner instead of inventing a price.

## When to use it

- Use it when generating a new magic item and the item needs a value.
- Do not assign a price if one is not needed.
- Do not apply it to items recorded from the owner's session notes. If a past item's value was not recorded, write "value not recorded."

## How to use it

1. Confirm the item's rarity. If it is not stated, ask.
2. Roll the dice yourself, for example by running a short script, and show the roll along with the result (for example, "Rare: 5d100 = 41 + 8 + 77 + 23 + 90 = 239 pp").
3. Record the result in the item's file under `worlds/<world>/items/`.
4. Do not invent other prices, ranges, or adjustments beyond this table.
