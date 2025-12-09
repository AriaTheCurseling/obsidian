!!! Learn

Hamming distance

p1 = 1 - r/d
p2 = 1 - cr/d

k is number of bits hashed
L is number of hash functions (independently selecting bits)

k = lg n / lg(1/p2)
ρ = lg (p1) / lg(p2)
L = ceil(2n^ρ)

insertion time kL
query time L(k+d)