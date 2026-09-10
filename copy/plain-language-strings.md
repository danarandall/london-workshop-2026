# Plain Language Strings

Use these exact words for any customer-facing text. When a value slots in, keep the currency symbol and format shown.

## Balances and headings

- Balance heading: "Available to spend"
- Balance sub-line: "£{available} available. £{pending} pending."
- Savings pot heading: "Rainy day"
- Section heading for transactions: "Recent activity"
- Empty transactions state: "No activity in the last twenty items."

## Buttons

- Primary action on dashboard: "Send money"
- Confirm on move-money form: "Send £{amount}"
- Cancel on any form: "Cancel"
- Retry after a failure: "Try again"
- Open thirty-day chart: "Show 30-day activity"
- Close thirty-day chart: "Hide 30-day activity"

## Form fields

- Payee field label: "Who are you paying?"
- Amount field label: "How much?"
- Reference field label: "Add a note (optional)"
- Required indicator (text, not colour): "Required"

## Statuses (in text; colour is reinforcement, never sole signal)

- posted: "Cleared"
- pending: "Pending"
- declined: "Declined"
- refund: "Refund"

## Failure and success

- Success: "Sent £{amount} to {payee}. Reference: {ref}."
- Insufficient funds: "We couldn't send £{amount} to {payee}. Your available balance is £{available}. Try a smaller amount, or move money in first."
- Invalid payee: "The sort code or account number for {payee} looks wrong. Check the details and try again."
- Network timeout: "We couldn't reach the bank. Your payment has not been sent. Check your connection and try again in a moment."
- Session warning: "You'll be signed out in one minute. Anything you've typed is safe. Do you want to stay signed in?"

## Words to avoid

- "Payment Failed" (no explanation, no next step)
- "Error"
- "Oops"
- "Invalid input"
- "Something went wrong"
- Colour-only status ("red = declined", "green = cleared")
