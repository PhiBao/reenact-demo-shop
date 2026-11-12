---
mode: testing
url: http://localhost:4100/
headless: true
max_steps: 30
tags: [reenact, issue-5]
---

# checkout is broken, please fix asap

## Reproduce the report
Open http://localhost:4100/.
Stay on localhost:4100 for the whole run and do not open any other website.
Do each step once, in order. If the app behaves unexpectedly, do not undo, retry, repair or work around it: the behavior itself is what is being checked. Check the result right after the last step.
Steps:
1. Open the cart page with the cart empty
2. Type SAVE10 into the coupon box
3. Click the Apply coupon button
The reporter says the correct behavior is that The Total does not show a negative amount (it does not show -$10.00); with an empty cart the Total is $0.00. Verify that The Total does not show a negative amount (it does not show -$10.00); with an empty cart the Total is $0.00.
