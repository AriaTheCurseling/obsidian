Each node has access to its own random number generator

monte carlo, fixed time, probabilistic success
las vegas, fixed success, probabilistic time

Randomized coloring using las vegas
- given an n-node graph if degree x
- output a x+1 coloring

Alternate steps:
setup
|C| = d+1

even round:
50% choose c from C
share c
collect shared values as N

odd rounds:
if c not in M
stop and share c
receive shared values as S
C = C / S

we want to stop with probability (1-1/n^C)
probability we haven't stopped 1/n^C
probability a node hasn't stopped 1/n^C+1

(3/4)^k=n^-(C+1)
k log(3/4) = -(C+1) log (n)
k = (C+1) log (n) / log(4/3)

time log n