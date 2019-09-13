#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  This is only going to run once, no matter what you put into it. The runtime complexity is O(1). Congratulations.


b)  This takes a process that runs at O(log2(n)), and runs it n times. So the complexity is O(n * log2(n)) 


c)  This makes a number of function calls equal to the argument passed into it, which is a linear relationship: O(n) 


## Exercise II

It seems that you are trying to find a single number, "f", out of a sorted list (a range from 0 to the top floor of the building). You could use a binary search for this one if you want to do fewer drops. But, since it seems like you're trying to minimize the amount of broken eggs, it would probably be prudent to just try the lower floors until your first egg breaks.

I propose this algorithm:

Let "n" start at 0.
While the number of eggs you have broken is 0:
    Go to floor "n" and drop an egg.
    If the egg breaks, you are on floor "f". Stop dropping eggs, please.
    Otherwise, add one to "n", and repeat this process.

This solution is effectively a linear search, and has a runtime complexity of O(n).
