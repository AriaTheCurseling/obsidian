A computer network given bby a graph computes properties about itself.
node id's in 0 .. n^d messages in 0 .. n^c where d is node count

Single-Source Shortest Path Distances
nodes initialized with:

if received message last round
send message
set distance to round nun
stop

Breadth-First Search
reply accept to random wave source
if all accepted children have acknowledged send acknowledge to parent

Electing a leader
- one node should output 1, all others 0
bfs but store root id instead of stopping
redo if smaller id is sent

All-Pairs Shortest Path Problem
