---
mode: testing
url: http://localhost:4100/
headless: true
max_steps: 30
tags: [reenact, issue-3]
---

# Quantity can go negative

## Reproduce the report
Open http://localhost:4100/.
Stay on localhost:4100 for the whole run and do not open any other website.
Do each step once, in order. If the app behaves unexpectedly, do not undo, retry, repair or work around it: the behavior itself is what is being checked. Check the result right after the last step.
Steps:
1. Open the coffee beans product in the store
2. Click the add to cart button for the coffee beans
3. Open the cart
4. Click the minus button next to the coffee beans once
5. Click the minus button next to the coffee beans a second time
6. Click the minus button next to the coffee beans a third time
7. Click the minus button next to the coffee beans a fourth time
The reporter says the correct behavior is that The coffee beans quantity never shows a negative number and the cart total is never negative; the quantity stays at 1 or the item is removed from the cart. Verify that The coffee beans quantity never shows a negative number and the cart total is never negative; the quantity stays at 1 or the item is removed from the cart.
