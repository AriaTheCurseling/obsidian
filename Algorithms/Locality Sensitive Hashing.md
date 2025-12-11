!!! Learn

delta-Probabilistic c-Approximate r-Near Neighbor
Hamming distance
b is byte count

p1 = 1 - r/b
p2 = 1 - cr/b

k is number of bits hashed
L is number of hash functions (independently selecting bits)

k = lg n / lg(1/p2)
ρ = lg (p1) / lg(p2)
L = ceil(2n^ρ)

insertion time kL
query time L(k+d)

probability that x and z collides given d(x,z) <= r
probability that 1 hash collides
P\[h(x) = h(y)] = (1-d(x, z)/b)^k 
probability that atleast one hash collide
1 - (1 - (1-d(x, z)/b)^k)^L 
1 - (1 - (1-p^k)^L 
1 - e^(Lp^k)

Jaccard Similarity
choose random elements to hash (so no different from hamming)

Angular Distance
Sim hash, choose random vectors, compare and use sign as bit value
