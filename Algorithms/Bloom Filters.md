###### Solves the membership problem
Given an element x and a set X of n elements, how do we efficiently determine if x is in X
###### Standard solution
Hash Set, time 1, space n, stores all elements according to hash
###### Probabilistic solution
A bloom filter will always correctly identify members, but can falsely claim non-members as members with some probability.

has k independent hash functions and m bits

the chance an individual bit is not set is (1-1/m)^(kn) which is approximately e^(-kn/m)

the false positive rate is given by the the probability k bits is in set is (1-p)^k = ( 1 - e^(-kn/m) )^k 

optimal k = ln2*(m/n)

using m = ceil(n * lg(1/error) / ln 2) and k = ceil (lg 1 / error) we can set the error





can be combined by bitwise or
can vhe
