

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


Heavy hitters problem
CountMin Sketch + min-heap + counter m

add each element in stream to sketch
check if element frequency is above m/k
if so, add to min-heap
remove lowest value in heap if its below m/k

space k * log 1/δ
time 


