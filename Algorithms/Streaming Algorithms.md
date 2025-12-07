Selection problem
Reservoir sampling
- we want to select a random element with uniform probability from a stream

Select each element with chance 1/n, replacing previous selection, where n is number of seen elements

Frequent elements Problem - Heavy Hitters Problem
- Find all elements that occour more than m/k times for some k
keep k - 1 counters
for each element either
- increment counter
- create counter at 1
- decrement all counters and remove 0 values

Distinct elements problem

Tidemark algorithm
- choose a 2-universal hash function
- keep track of max(count_trailing_zeros(hash(x))) as z
- return 2^(z+1/2)
!! learn the bounds

Approximate counting problem

Morris counter
- initialize x as 0
- with probability 2^-x increment x
- output 2^x - 1

Morris counter (space inneficient)
- initialize x as 1
- with probability 1/x bitshift x << 1
- output x - 1
