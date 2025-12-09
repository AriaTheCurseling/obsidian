Streaming the edges m of a graph
vertices n are known


Graph Connectivity Problem
connected = false
forest = {}

For each edge:
- if forest union edge doesn't have cycles set forest to the union
- if size of forest equals n-1 set connected true

Size n,  or n log n bits

Bipartiteness problem
bipartite = true
forest = {}

For each edge:
- if forest union edge doesn't have cycles set forest to the union
- else if forest union edge has an odd cycle set bipartite = false

Size n,  or n log n bits

Distance Problem
t-Spanner Edge Property

subgraph = {}

for each edge:
if d(x, y) >= t + 1 append edge to subgraph

space n^(1+2/t) log n bits
