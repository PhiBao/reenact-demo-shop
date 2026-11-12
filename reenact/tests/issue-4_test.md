---
mode: testing
url: http://localhost:4100/
headless: true
max_steps: 30
tags: [reenact, issue-4]
---

# Remove button deletes the wrong item

## Reproduce the report
Open http://localhost:4100/.
Stay on localhost:4100 for the whole run and do not open any other website.
Do each step once, in order. If the app behaves unexpectedly, do not undo, retry, repair or work around it: the behavior itself is what is being checked. Check the result right after the last step.
Steps:
1. Add the enamel mug to the cart
2. Add the coffee beans to the cart
3. Open the cart
4. Click the Remove button on the coffee beans row
The reporter says the correct behavior is that after clicking Remove on the coffee beans row, the cart no longer shows the coffee beans and still shows the enamel mug. Verify that after clicking Remove on the coffee beans row, the cart no longer shows the coffee beans and still shows the enamel mug.
