Input is n elements stored arbitratily in M = Cn/S machines.
Each machine has S = n^epsilon memory
C >= 2, epsilon > 0

Sorting problem
Quicksort algorithm
select pivots with probability p = (n^epsilon/2)/2n, with high probability less than n^epsilon/2 elements

gather all elements in 1 machine and sort

broadcast sorted list over 1/epsilon rounds using a broadcast tree

convergecast intervals

central decides which machines are responsible for each interval (broadcast intervals)

randomly distribute to correct computers

recurse on each subproblem


with probability 1-n^-10 it is solved in 1/epsilon^2 



Minimal Spanning Forest Problem
E' = E
recursively
- fit E' into as few nodes as possible
- each node calculates local msf(E')
- E' = msf(E')
as long as more edges can fit in machine memory than the maximal spanning forest, this will converge on the solution




