Input is n elements stored arbitratily in M = Cn/S machines.
Each machine has S = n^epsilon memory
C >= 2, epsilon > 0


Quicksort algorithm
select pivots with probability p = (n^epsilon/2)/2n, with high probability less than n^epsilon/2 elements

gather all elements in 1 machine and sort

broadcast sorted list over 1/epsilon rounds using a broadcast tree

convergecast intervals





Sorting problem
variant of quicksort
probibalistic

send random elements to 1 computer
it sorts those and returns their order 
count how many elements in between each sorted element
sum counts
??? 
profit

Minimal Spanning Forest
E' = E
recursively
- fit E' into as few nodes as possible
- each node calculates local msf(E')
- E' = msf(E')
as long as more edges can fit in machine memory than the maximal spanning forest, this will converge on the solution




