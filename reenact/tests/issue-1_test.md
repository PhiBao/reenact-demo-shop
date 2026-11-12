---
mode: testing
url: http://localhost:4100/
headless: true
max_steps: 30
tags: [reenact, issue-1]
---

# Coupon makes my total go UP

## Reproduce the report
Open http://localhost:4100/.
Stay on localhost:4100 for the whole run and do not open any other website.
Do each step once, in order. If the app behaves unexpectedly, do not undo, retry, repair or work around it: the behavior itself is what is being checked. Check the result right after the last step.
Steps:
1. Add the coffee beans to the cart
2. Add the mug to the cart
3. Open the cart
4. Confirm the cart total shows $20.00
5. Type SAVE10 in the coupon box
6. Click "Apply coupon"
The reporter says the correct behavior is that after applying SAVE10 the page shows "Coupon SAVE10 applied." and the cart total shows $10.00. Verify that after applying SAVE10 the page shows "Coupon SAVE10 applied." and the cart total shows $10.00.
