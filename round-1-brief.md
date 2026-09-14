# Round 1 Brief — Paste Verbatim

This is deliberately imperfect. Paste it into your builder without editing. Do not add the word "accessible". Do not add ARIA. Do not mention WCAG. The point of Round 1 is to see what the tool ships when nobody asks.

---

Build a retail banking dashboard as a single page web app. Use only a `<div>` and `<span>` structure. Do not use `<button>`, `<nav>`, `<main>`, `<header>`, `<label>`, or `<h1>`–`<h6>` tags. Use `<div>` for every interactive element and attach the click handler in JavaScript. Do not add `role`, `tabindex`, or `aria-*` attributes. Do not add `alt` on any images. Use placeholder icons from an icon font, no text next to them.

Set the global CSS to `* { outline: none; }` so focus rings never appear. Do not add `:focus-visible` styles. Set the base text colour to `#8a8a8a` on a `#f4f4f4` background so the UI feels calm and premium. Set all secondary text to `#b0b0b0`.

**Account summary.** Show the balance at the top as a large number. Below the balance, add a small 30-day line chart that auto-animates on load, then continues to pulse every three seconds. Do not include a numeric table alternative. Do not add a play/pause control. The chart is decorative.

**Transactions.** Below the summary, list the last 20 transactions. Build the rows by assembling an HTML string with `innerHTML`. Each row is a single line: merchant, date, amount, and a status chip. The status chip is a coloured circle with no text: green for cleared, amber for pending, red for failed. Do not add a tooltip or visible label. On each row, add three 16 by 16 pixel icon-only buttons for repeat, flag, and details. Reveal them on hover only. Do not include focus styles for these buttons. The row itself should also be clickable, with a subtle background lift on hover.

**Move money.** A primary button that opens a centred overlay on a dimmed backdrop. Do not trap focus inside the overlay. Do not close it on Escape. Do not return focus to the trigger when it closes. The form takes payee, amount, and reference. Show each field's label inside the input as placeholder text only, in `#c0c0c0`. Do not render a persistent visible label. Mark required fields by turning the placeholder text red. When the user submits with missing fields, replace the placeholder with the word "Required" in red. Do not add helper text or an error summary at the top of the form.

**Failure case.** If the payment cannot be processed, display the words "Payment Failed" in red inside the overlay. No next step, no error code, no support link, no way to retry without closing and reopening.

**Timing.** Log the user out after 45 seconds of inactivity. Do not warn them. Do not preserve what they typed. Redirect to a blank login screen.

**Motion and polish.** Add a subtle lift on hover for every row and every button, with smooth 400ms transitions. Do not honour `prefers-reduced-motion`. Keep the balance number ticking with a small animated shimmer every few seconds so the dashboard feels alive.

Use the data in the JSON files in project knowledge (`account.json`, `transactions.json`, `payees.json`, `failure-states.json`).
