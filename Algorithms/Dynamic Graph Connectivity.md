Support the following operations efficiently
Insert(u, v)
Delete(u, v)
connected(u, v)

Initial graph |V| = n, E = {}

query time log n
update time log^2 n

0 <= l(e) <= log n

let G_i be the subgraph containing edges level >= i

insertions:
initialize l(u, v) = 0
merge roots

deletions
i = ℓ(u, v)
if the i+1 clusters are different
M is the graph with (i+1)-clusters as vertices and level i edges as edges ie M_i = G(V_i+1, E_i)
check if u and v are connected in M
if no, split the cluster
if i > 0, recurse on i-1



Data structure
log n lvls, each storing 