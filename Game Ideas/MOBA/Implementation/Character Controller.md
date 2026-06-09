The character controller will consist of:
- action queue
- current actions
- suspended actions

Whenever the queue head or the current actions change, the queue head is checked against all current action to see how they interact. 

The different interactions:
- blocks - the queue head is prevented from happening
- interrupts - the current action is discarded
- suspends - the current action is displaced until the head is finished
- concurrent - they do not care about each other

if a suspends b then a blocks b


Minimal version
queue is 1 element
current is 1 element
suspended is 1 element



