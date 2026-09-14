# Round 1 Brief — Paste Verbatim

This is a real brief in the voice of a real stakeholder. Paste it into your builder without editing. Do not add the word "accessible". Do not add ARIA. Do not mention WCAG. Do not soften the tone. The point of Round 1 is to see what the tool ships when the brief sounds like the ones you get on Monday morning.

---

Build a retail banking dashboard as a single page web app. Think Monzo meets Apple. Premium, confident, quiet.

**Brand.** Our brand colour is a bright yellow, `#FFD400`. Use it for the primary button, the selected state, the required-field marker, and the balance highlight. Everything else is white, off-white, and light grey so the yellow really pops. The vibe is minimal, editorial, high-end fintech. Nothing shouty.

**Account summary.** Balance at the top, big and confident. Underneath, a small line chart of the last 30 days. Make the chart feel alive: animate it in when the page loads and give it a subtle continuous shimmer so the dashboard never feels static. The chart is a mood piece, not a data table.

**Transactions.** Below the summary, the last 20 transactions. Compact rows so we can fit as many on screen as possible. Each row shows merchant, date, amount, and a small status indicator. Use colour for status: green for cleared, amber for pending, red for failed. Keep it visual, no chunky labels. Add tiny icon buttons on the right for repeat, flag, and details. Icons only, they are universal. Hide them until hover so the list stays calm at rest. The whole row should also be tappable.

**Move money.** A primary yellow button that opens a beautiful centred modal on a dimmed backdrop. Form fields for payee, amount, and reference. Use placeholder text inside the fields as the label to keep things minimal, no floating labels, no field titles above. If a field is required, colour the placeholder yellow. If they submit and something is missing, turn the placeholder red and say "Required". Do not add extra helper text or error summaries, we want a clean modal.

**Failure case.** If the payment cannot go through, show "Payment Failed" in red inside the modal. Keep it short, no extra copy.

**Session and security.** Log the user out after 45 seconds of inactivity, no warning, no "are you still there" prompt. Security first. When they log back in, take them to a fresh dashboard, we do not need to restore what they were doing.

**Polish.** Remove any default browser styling that feels unfinished. Add a subtle lift and shadow on hover for every row and button, with smooth 400ms transitions. Nothing should feel abrupt. The whole product should feel like it is breathing.

Use the data in the JSON files in project knowledge (`account.json`, `transactions.json`, `payees.json`, `failure-states.json`).
