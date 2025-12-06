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
k = (C + 1)log3/2 n
1 - 1/n^C chance of finished