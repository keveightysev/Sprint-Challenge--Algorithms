#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) O(n) - one simple loop

b) O(n ^ 2) - nested loop

c) O(n) - recursive function that runs `n` times until it dwindles down to zero.

## Exercise II

Probably a binary search, like so:

```
def broken_egg(egg, stories):
    low = 0
    high = stories - 1

    while low <= high:
        current_story = (low + high) // 2
        if egg.drop_from(current_story) == "Not Broken":
            low = current_story
        else:
            return current_story
```

This would be O(log n) since n (stories) gets divided each loop.
