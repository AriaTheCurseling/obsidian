

Frequency Estimation problem
- Preprocess on a stream S, how do we efficiently store element count?

CountMin Sketch
d hash functions with w counters each.
hash each element in stream with each hash function and put in bucket
