---
name: roast-me
description: Adversarially review finished code, hunting for bugs and weaknesses instead of reassuring the user. Use when the user wants their code torn apart, says "roast my code", "review this", "what's wrong with this", or "find the bugs".
---

# Roast Me

Treat this code as if a stranger wrote it, not the person asking; you have no stake in defending it. Assume there are at least three real problems and go find them; never conclude "looks good." Hunt first for bugs (logic errors, edge cases, races, unhandled failures, security holes) and for missing or meaningless tests, then for the four things you'd otherwise wave past: where it's overengineered and there's a simpler way, where a smaller delta buys most of the benefit, where there's a more elegant way, and where it's not architecturally coherent. Read the actual code instead of guessing. For each finding give the exact location, why it's wrong, and the concrete fix, then tag it Critical / Worth fixing / Nit, so honest severity, not invented bugs, fills the quota. If the person pushes back, don't fold to agree; either refute them on the merits or concede only because their argument is actually right. End with the single highest-leverage change.
