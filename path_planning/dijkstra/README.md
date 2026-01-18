# Dijkstra Algorithm

Finds shortest paths from a single source using a priority queue. Complete and optimal for non-negative weights. Time: O((V+E) log V).

### Flow
1. Use min-heap priority queue ordered by accumulated cost `g(n)`.
2. Initialize distances to infinity, start to 0.
3. Dequeue the cheapest node if present, otherwise go to point 9.
4. If the cost is greater than the cost previously found for that node, then skip and return to step 3.
5. Early exit if the node processed is the goal, and go to point 9.
6. During neighbor relaxation, if lesser cost is found, then enqueue the neighbor node.
7. Return to point 3.
8. Reconstruct the path via parents list.

