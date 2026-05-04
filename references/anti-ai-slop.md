# Anti-AI-Slop Guide

Your design must NOT look AI-generated. AI interfaces converge on the same tired patterns because they optimize for "safe" and "average." Real designers make intentional, contextual choices.

---

## 🚨 THE #1 TELL: INDIGO/VIOLET

Every AI model defaults to indigo/violet (`#6366f1`, `#8b5cf6`, `#7c3aed`). It's the universal fingerprint of AI-generated design.

Why it happens: training data saturated with Tailwind's indigo. LLMs optimize for the average, and indigo IS the average.

**RULE: NEVER use indigo/violet unless the brand explicitly requires it.**

| Instead of | Try | Feeling |
|------------|-----|---------|
| Indigo `#6366f1` | Blue `#2563eb` | Trust, professional |
| Violet `#8b5cf6` | Teal `#0d9488` | Fresh, distinctive |
| Purple `#7c3aed` | Brand color | Authentic, intentional |

---

## 🚨 THE #2 TELL: CARDS EVERYWHERE

Cards are the second most common AI-slop pattern. AI models wrap everything in rounded-corner boxes with shadows because it feels "safe." Real designers use cards sparingly.

**RULE: Default is NO cards. Use sections, columns, dividers, or media blocks instead.**

Cards are only justified when they are the container for a user interaction (clickable item, form, expandable panel). If removing the border, shadow, background, or radius doesn't hurt interaction or understanding — it's not a card, remove it.

Ask: "Is this a card because the user needs to interact with this container, or because I couldn't think of another way to group things?" If the latter — remove the card.

---

## 🚨 THE #3 TELL: DARK MODE BY DEFAULT

AI models default to dark backgrounds. Dark-by-default is an AI fingerprint just like indigo.

**RULE: Unless the brief explicitly asks for dark — use light mode.**

Dark mode is a deliberate brand choice, not a default. When a brief says nothing about color mode, light mode is the professional baseline.

---

## 🚨 THE #4 TELL: EMOJI AS ICONS

Standard emoji (😀🚀💡🎯) immediately signal "AI-generated." They're a shortcut that makes any design look cheap and unfinished.

**RULE: Never use emoji unless the user explicitly asks for them.**

Use instead: icon libraries (Lucide, Phosphor, Heroicons), Unicode symbols (→ • ◆), SVG graphics. Even a simple text character beats a yellow smiley in a professional UI.

---

## 🚨 THE #5 TELL: LEFT ACCENT STRIPE

The colored vertical bar on the left edge of a card (`border-left: 4px solid <accent>`). AI models add it for "visual interest" — but in shipped products this stripe is reserved for elements that carry meaning: callouts, alerts, active list items, status, priority.

**RULE: Only use a side accent stripe when it communicates something — status, priority, owner, or selection. Never as decoration.**

If you can't say in one word what the color means, remove the stripe.

---

## What Makes Design Look Generic

**Typography symptoms:**
- Same font as every other AI site, same weight throughout
- No distinction between display and body text
- Missing letter-spacing on ALL CAPS and small text

**Color symptoms:**
- Default indigo/violet, gradients that don't serve function
- Perfectly even color distribution, no clear accent hierarchy

**Layout symptoms:**
- Perfectly symmetrical everything, cookie-cutter card grids
- Hero with left text + right image (every landing page ever)
- Centered everything with no visual tension

**Visual symptoms:**
- Abstract blob backgrounds, generic 3D illustrations
- Effects without purpose, stock imagery that could be anywhere

---

## The Antidote: Intentional Design

**Typography with purpose:**
- Choose fonts that match your tone from research
- Create clear hierarchy (3-4 distinct levels)
- Use weight and spacing to differentiate, not just size

**Color with meaning:**
- Build palette from references, not defaults
- Use dominant + sharp accent, not evenly distributed
- Make semantic colors actually semantic

**Layout with intention:**
- Create visual tension through asymmetry
- Use whitespace as a design element
- Break the grid intentionally (one element, not everything)

**Details that distinguish:**
- Custom illustrations or real photography
- Micro-interactions that reinforce brand
- Shadows and depth when they serve hierarchy
- One memorable detail users will actually remember

---

## The AI Slop Detector Checklist

Before shipping any design:

```
□ Accent color is NOT indigo/violet
□ Cards are justified by interaction, not used as default containers
□ No decorative left/side accent stripes
□ No standard emoji used as icons
□ Color mode is light unless brief explicitly asks for dark
□ ALL CAPS text has letter-spacing
□ Would pass the "screenshot test" next to real products
□ Font choices are intentional and contextual
□ Colors derived from research, not defaults
□ Layout has visual interest and tension
□ No generic patterns you can't justify
□ You can explain WHY each design choice was made
```

---

## Litmus Tests

Run these against your design before shipping:

**Card test:** If removing border + shadow + background + radius doesn't hurt interaction or understanding → it's not a card, remove it.

**Image test:** If the first viewport works fine without the hero image → the image is too weak. Make it dominant or remove it.

**Brand test:** If the brand disappears after hiding the nav → hierarchy is too weak. Make brand louder — bigger logo, brand color in hero, distinctive typography.

**Copy test:** If deleting 30% of copy improves the page → keep deleting. AI over-writes; real designers edit down.

**Identity test:** If the first viewport could belong to any other company → branding is too weak. Add the one detail that makes this unmistakably THIS brand.

---

## Safe vs. Intentional

Safe (forgettable):
- 3-column pricing because "everyone does it"
- Hero with left text + right image because "it works"
- Card grid with equal spacing because "it's clean"

Intentional (memorable):
- 2-column pricing because your product only has 2 tiers
- Full-width hero image with overlay because it fits the brand
- Asymmetrical layout because you want visual tension

"I chose this because [specific reason for THIS project]" beats "I chose this because everyone does it."
