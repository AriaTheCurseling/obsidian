Given an undirected graph G with non-negative edge weights, we want a data structure that answers queries for δ(u, v) for vertices u, v, where δ(u, v) is the shortest path distance in G between u and v.

Estimate distances at a certain stretch

Given a graph G(E, V)

randomly sample verticies with probability p
for each vertex store the distance to everything closer than the closest sampled vertex
for each vertex store the distance to each sampled vertex
for each vertex store the closest sampled vertex 

randomly sample vertices

amount of samles is n * p
stored in n * n * p
expected vertices closer than sampled vertex order of 1/p (geometric distribution)
strored in n/p

set p to sqrt(n) and stored in n sqrt n


recursively applying algorithm to previous sample

Each vertex:
closest stored in 1/p for every layer, total k/p
last layer size expected np^k-1
each layer closest vertex

total size nk/p + nnp^k-1
using p=n^-1/k
we get kn^(1+1/k)

