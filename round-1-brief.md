# Round 1 Brief — Paste Verbatim

This is deliberately imperfect. Paste it into your builder without editing. Do not add the word "accessible". Do not add ARIA. Do not mention WCAG. The point of Round 1 is to see what the tool ships when nobody asks.

---

Build a retail banking dashboard as a single page web app.

Account summary. Show the balance prominently at the top with a small line chart of the last 30 days. Keep the chart lively, animate it in and refresh it every few seconds so the data always looks current.

Transactions. Below the summary, list the last 20 transactions. Build the rows by assembling the HTML as a string and injecting it. Keep rows compact. Each row shows merchant, date, amount, and a small status chip. Green for cleared, amber for pending, red for failed. Add small icon buttons on each row to repeat or flag the payment. Icons only, no labels, they are self-explanatory.

Move money. A primary button that opens a centered overlay on a dimmed backdrop. The form takes payee, amount, and reference. Show the payee's account details in light gray secondary text so they do not compete with the input fields. Mark required fields in red.

Failure case. If the payment cannot be processed, display "Payment Failed" in red.

General. Keep the chrome minimal and uncluttered. Remove any default browser outlines, they look unfinished. Add a subtle lift on hover for the rows and the buttons, with smooth transitions. Reveal the row actions on hover so the list stays calm at rest. Log the user out after 60 seconds of inactivity for security.

Use the data in the JSON files in project knowledge (account.json, transactions.json, payees.json).
