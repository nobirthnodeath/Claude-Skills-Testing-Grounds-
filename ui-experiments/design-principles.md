# Kitchen app: visual design principles

Scope: the look and feel of Home and Inventory. The light theme comes from Fresh Picks and the dark theme from Evening Kitchen. The theme follows the phone setting. Features and tasks do not change.

Who uses it: mostly moms, also dads and roommates. They plan dinner, add to the grocery list, and shop in the store.

## Principles, in priority order

When two principles conflict, the higher one wins.

### 1. A tool first, a friend second

**Statement.** The app helps people waste less food and save money. It must look calm and capable. Warmth is welcome, but play is not.

**Why.** People trust a tool with their money. A toy-like look makes the numbers feel less serious.

**Do.** Use a plain, well-made sans serif, straight edges with a moderate radius, and short, direct copy.

**Don't.** Use rounded "bubbly" fonts, tilted stickers, pastel blocks on every section, or exclamation marks.

**Trade-off.** Less instant delight. We get it back through warm color and kind copy, not through decoration.

### 2. Color means something

**Statement.** Red means expiring or expired. Green means good news. Everything else stays neutral, so these two colors always stand out.

**Why.** If red and green also decorate, users can no longer trust them as signals.

**Do.** Use a neutral base and dark ink. Use green for primary actions and for good news ("used"). Use red only for "today", "expired" and the expired alert. Give the cook card its own soft cool tint (periwinkle), not green and not red.

**Don't.** Use yellow anywhere. Give food groups strong colors, or use red for anything that is only "important".

**Round 6 change.** Green was first kept only for good news. It is now the primary action color, by your choice. Good news and actions are both positive, so they can share it.

**Trade-off.** Food groups are harder to tell apart by color. They are told apart by headings and icons instead.

### 3. Readable at the stove and in the aisle

**Statement.** Every screen must be easy to read at arm's length, with one hand, in bright store light or a dim kitchen.

**Why.** People use the app while cooking and shopping, not sitting at a desk.

**Do.** Use 16px or larger for item names, strong contrast in both themes, tap targets of 44px or more, and fixed-width numbers in columns.

**Don't.** Use light-gray small text for anything people need to act on, or make the dark theme a simple inversion of the light one.

**Trade-off.** Fewer items fit on one screen.

### 4. Soften the hard moments

**Statement.** Waste and expired items are facts, not failures. Say them clearly and calmly, and always show the next step.

**Why.** The airy feel exists to make "you tossed $17 this week" feel easier to face, so the user keeps using the app.

**Do.** Use a plain sentence, a quiet layout around the number, and one clear action ("Sort them").

**Don't.** Use a full red block, alarm icons, or guilt words ("wasted", "failed").

**Trade-off.** The alert is less loud. The red count and its position at the top keep it visible.

### 5. Numbers, not charts

**Statement.** Show the number and say what it means. Add a chart only when it shows something the number cannot.

**Why.** The "typical week" amount changes over time. A bar or a row of circles with it as a fixed full length suggests a precision we do not have.

**Do.** Write "2 things, about $9" and "Usually about 5 things, $22."

**Don't.** Draw bars, rings or filled circles against the typical-week number on Home.

**Trade-off.** Home is less visual. Type size and layout carry the weight instead.

### 6. Space before boxes

**Statement.** Mark sections with space, headings and rules first. Use a card only for an object people act on.

**Why.** A card on every section makes all sections look equally important, and the screen looks busy.

**Do.** Use full-width lists with hairline rules and large section headings. A soft background band is fine for one key section.

**Don't.** Put every section in a white rounded card with a shadow.

**Trade-off.** Groups of content need careful spacing to stay clear.

**Round 3 decision.** Home has no cards except the cook prompt. That card is one tappable row with a right chevron and no large button inside it. In dark themes, depth comes from soft gradients and slightly see-through layers (the cook card and the tab bar). Keep these effects faint enough that a screenshot in grayscale still reads the same.

## Check against earlier rounds

| Earlier choice | Principle | Result |
|---|---|---|
| Sorbet: rounded font, tilted "today!" sticker | 1 | Fails. Too playful. |
| Market Stall: strong color for each food group | 2 | Fails. Competes with red and green. |
| Fresh Picks: green as the brand color | 2 | Passes after the round 6 change. |
| Fresh Picks and Evening Kitchen: bar or circles against "typical" | 5 | Fails. The benchmark changes. |
| Evening Kitchen: freshness dots on every row | 5 | Mostly fails. The day count already says it. |
| Evening Kitchen: warm dark surfaces, butter-yellow actions | 1, 2, 3 | Passes. Keep. |
| Fresh Picks: food-group icons in neutral tiles, red only for "today" | 2 | Passes if the tiles stay neutral. |
| Fresh Picks: kind message on quiet weeks | 4 | Passes. Keep. |
