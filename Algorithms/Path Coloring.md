P3C - 3 colors, undirected:
Generate random unique id.
Share id with neightboors
If highest local id, set to lowest unique value

faster deterministic path coloring - directed graph
generate random unique id
share id in direction
find the bit where received and own id differ
set own id = 2 * bit_index + bit_value
when reaching 6 colors use P3C

Randomized path coloring
all non-stopped nodes pick a color
share colors
if new color is different than neighbors, stop

we want probability that all nodes have stopped = 1 - 1/n^C
this means probability that a node has not stopped must be 1/n^(C+1)
(2/3)^k = n^-(C+1)
k log(2/3) = -(C+1) log n
k = -(C+1) log n / log(2/3)
k = (C+1) log n / log(3/2)

!! read up on math

