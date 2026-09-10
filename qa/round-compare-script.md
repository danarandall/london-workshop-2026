# Round Compare — Ten Checks

Run this against the Round 1 build, then the Round 2 build. Score each check pass or fail. Do not fix as you go; note it and move on.

1. **Focus is visible.** Tab through the whole page. Every focusable element shows a clear focus style. Fail if any focus disappears.
2. **Keyboard only.** Complete a Send Money without touching the mouse. Fail if any step requires a click.
3. **Escape closes the form.** Open Send Money, press Escape. Fail if the form stays open or focus does not return to the button that opened it.
4. **Focus is trapped in the open form.** Tab from the last field. Fail if focus leaves the form before it closes.
5. **Status is in text.** Read the transactions list without seeing colour (squint or turn to greyscale in devtools). Fail if you cannot tell posted from declined.
6. **Required fields marked in text.** Look at the Send Money form. Fail if required is signalled only by an asterisk in a coloured label.
7. **Failure has plain language and a next step.** Trigger insufficient funds. Fail if you see "Payment Failed", "Error", or a message with no action.
8. **Balance is the focal point.** Squint at the dashboard. Fail if the balance is not the first thing you see.
9. **Motion is opt-in.** Load the page. Fail if anything moves, refreshes, or animates on its own before the user asks.
10. **Touch targets.** Measure any row action. Fail if under 24 by 24 CSS pixels. Note if under 44 by 44.

## Scoring

Round 1 score: __ / 10  
Round 2 score: __ / 10  
Delta: __

The delta is the point of the workshop. Not the absolute number.
