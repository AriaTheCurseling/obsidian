

Frequency Estimation problem
- Preprocess on a stream S, how do we efficiently store element count?

CountMin Sketch
d hash functions with w counters each.
hash each element in stream with each hash function and put in bucket

Using w = 2/ε and d = lg(1/δ)

upper bound on estimate is true value + εm with probability δ

space O(lg(1/δ)/ε)
time  O(lg(1/δ))
!! read up on calculations

Range Upgrade
Use log n countMin sketches, each hashing in bigger groups (ie, ignoring 1 extra significant bit)





