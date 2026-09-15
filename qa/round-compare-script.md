# Round Compare — Ten Checks

Run this against your Round 1 build, then your Round 2 build. Score each check pass or fail. Do not fix as you go. Note it and move on. The delta between the two rounds is the point.

Eight of these ten need a human. Two are machine detectable. That gap is the reason a human still runs QA.

## The ten checks

1. **Keyboard tour.** Tab from the top of the page to the bottom. You can reach every control, focus never disappears, focus is always visible, and the tab order matches what you see on screen. Human.
2. **Icons have words.** Look at every icon-only button and row action without hovering. You can tell what each one does from what is on screen. If you cannot tell a repeat from a flag from a details button, the label is missing. Human.
3. **Task without a mouse.** Complete a Move money end to end without touching the mouse. Open the modal, fill the fields, submit, close. Human.
4. **Colour is never the only signal.** Set the OS to grayscale, or a colourblindness simulator to Deuteranopia. Posted, Pending and Declined are still readable. Required is a word, not a colour. Human.
5. **4.5:1 text contrast.** Body text meets 4.5:1 against its background. Large text and UI components meet 3:1. Machine.
6. **24 by 24 touch targets.** Row actions and small controls measure at least 24 by 24 CSS pixels. Note anything under 44 by 44. Machine.
7. **Focus trapped and returned.** Open the Move money modal. Focus moves into it, stays inside it, and returns to the trigger on close or Escape. Human.
8. **Motion respects reduced-motion.** Load the page with reduced motion on. Nothing moves, refreshes, or animates before the user asks for it. Human.
9. **Plain-language errors that tell you what to do.** Trigger insufficient funds. The message names what happened and what to do next, in the same breath. No "Payment Failed". No "Error" with no action. Human.
10. **Session that warns before it ends.** Idle for the timeout. The app warns before signing you out, tells you your typed values are safe, and offers to stay signed in. Never silently logs you out mid-transaction. Human.

## Scoring

Round 1 score: __ / 10
Round 2 score: __ / 10
Delta: +__

The delta is the point. Not the absolute number. The gap is what a rules file plus a plain-language brief buys you, without writing a line of code.
