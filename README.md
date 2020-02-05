# What is Dynamic Programming?
It is the way of solving the an optimal based on the sequence of decisions, each decision is a subproblem which are alike in nature.

## You can climb one or two steps with one step. How many different ways can you climb n staris?
Ans: f(n) = f(n-1)+f(n-2), where f(1) = and f(2)=2
### Python solutions
def number_of_ways_to_cross_the_stairs(n):
    if n==1:
        return 1
    elif n==2:
        return 2
    else:
        return number_of_ways_to_cross_the_stairs(n-1) + number_of_ways_to_cross_the_stairs(n-2)
