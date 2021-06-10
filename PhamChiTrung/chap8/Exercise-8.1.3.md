# Exercise 8.1.3:

# Write the predicate (only the predicate) to represent the requirement: 
* “List all the wireless mice that either retail for more than $100 or for which the store has more than 20 items.<br>
Also list non-wireless mice that retail for more than $50.”

```
The predicate describing whether to list a given mouse is:
((mouseT ype = wireless) ^ ((retail > 100) _ (stock > 20)))_
(:(mouseT ype = wireless) ^ (retail > 50))

```
