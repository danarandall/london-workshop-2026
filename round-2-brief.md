# Round 2 Brief — Paste After You Install the Rules File

Rules file installed from project knowledge. Start a fresh project or new chat before you paste this brief.

---

Build a retail banking dashboard as a single page web app. The person using this may be anxious, distracted, or interrupted. Design for calm.

**Account summary.** The balance is the single focal point of the screen. One clear number, generous space around it. Offer the thirty day activity as a chart the user can choose to open, not something that competes on arrival. The chart updates when the user asks it to, never on its own.

**Transactions.** The last twenty transactions. Each row carries merchant, date, amount, and status. Status is in text, with colour as reinforcement, never as the only signal. Rows are comfortable rather than compact. Every control is at least 24 by 24 CSS pixels, 44 by 44 preferred. Row actions are always present and reachable, not revealed on hover. Every control has a name that says what it does and which transaction it acts on.

**Move money.** One primary action, labelled in plain language. Advanced options such as wire or scheduled payment are revealed when the user needs them. When the form opens, move focus into it, keep focus inside it, close it on Escape, and return focus to the button that opened it. Required fields are marked in text, not by colour alone.

**Failure case.** If the payment cannot be processed, say so in plain language, explain what to do next, and announce it to assistive technology. Do not say "Payment Failed".

**Timing.** If a session must expire, warn well before, allow the user to extend it, and never lose what the user typed.

**General.** Focus must always be clearly visible. Reduced motion is a primary experience, not a fallback. Follow the accessibility rules in the project.

Use the data in the JSON files in project knowledge. Use the plain language strings file for any customer-facing text.
