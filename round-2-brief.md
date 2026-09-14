# Round 2 Brief — Paste After You Install the Rules File

Rules file installed from project knowledge. Start a fresh project or new chat before you paste this brief. Read `account.json` and `failure-states.json` before you build anything.

---

Build a retail banking dashboard as a single page web app. The person on the other side of this screen is Sam Okafor. Sam uses a screen reader sometimes and their eyes the rest of the time, prefers reduced motion, and banks in short bursts between other things. Sam is not new to banking, is not performing a special-needs task, and is not the exception. Sam is the customer.

Design for calm. Calm means the screen tells Sam what they need to know before they have to ask. Calm means nothing moves that Sam did not ask to move. Calm means Sam can get pulled away, come back five minutes later, and pick up where they were. Calm means when something goes wrong, the app says what happened and what to do next, in the same breath, in Sam's language.

**Brand.** Our brand colour is a bright yellow, `#FFD400`. Use it where a person's eye needs to land: the primary action, the current selection, the confirmation moment. Not for text on white. Not as the only signal that a field is required. If yellow is the only thing carrying meaning, meaning is missing.

**Account summary.** Balance at the top. One number, generous space, the largest thing on the screen. Show the currently available balance and the pending amount separately, in plain words, so Sam does not have to do maths to know what they can spend. The thirty day activity chart is a secondary view Sam can open, not something that greets them. When the chart is open it responds to Sam, it does not animate on its own.

**Transactions.** The last twenty transactions, one per row. Merchant, date, amount, status. Status is a word first and a colour second. Posted, Pending, Declined. Rows are comfortable to tap with a thumb and comfortable to read at arm's length. Every control has a name that describes the action and the transaction, so Sam's screen reader says "Repeat payment to Thames Water on 8 September" not "button". Row actions are always visible. Hover is not a feature we can rely on.

**Move money.** One primary yellow button, labelled in plain language. When the form opens, focus moves into it, stays inside it, and returns to the trigger when Sam closes it or presses Escape. Every field has a persistent visible label above the input. Required is a word, not a colour. If Sam submits with something missing, the top of the form summarises what is missing and links to each field. Sam's typed values are preserved through every state change.

**Failure case.** If a payment cannot go through, use the `recommended_message` from `failure-states.json` for that state. When Sam tries to send more than their available balance to Landlord Ltd, the message says exactly how much they can send and offers to adjust the amount, not "Payment Failed". The message is announced to assistive technology at the moment it appears, not only shown. Every failure carries a primary and secondary action that match the recommended actions in the data.

**Session.** Follow the `fail_session_expiring` behaviour in `failure-states.json`. Warn Sam one minute before sign-out, tell them their typed values are safe, and offer to stay signed in. Never silently log Sam out mid-transaction.

**Motion.** Reduced motion is the default experience for Sam, because Sam's profile says so. Motion is an opt-in flourish, not a baseline. Focus indicators are visible everywhere focus can land, at the moment focus arrives.

Follow the accessibility rules in the project. Use the data in the JSON files in project knowledge. Take every customer-facing sentence from `failure-states.json` where one exists, and match its tone everywhere else.
