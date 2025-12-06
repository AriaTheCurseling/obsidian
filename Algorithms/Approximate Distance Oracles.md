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