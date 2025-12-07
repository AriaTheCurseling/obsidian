Selection problem - Reservoir sampling
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