# Reverse-delete algorithm

↑ **Parent:** [Minimum spanning tree](minimum-spanning-tree.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reverse-delete_algorithm)

Process [edges](edge-of-a-graph.md) in decreasing weight and delete an [edge](edge-of-a-graph.md) whenever the remaining [graph](graph-split.md) stays connected. Previously retained heavier [edges](edge-of-a-graph.md) are [bridges in a graph](bridge-graph-theory.md) and remain so under deletion. Thus a deletable [edge](edge-of-a-graph.md) is heaviest on a current [graph cycle](cycle-in-a-graph.md), and the [minimum spanning tree cycle property](minimum-spanning-tree-cycle-property.md) excludes it from every [minimum spanning tree](minimum-spanning-tree.md). At termination the surviving connected [graph](graph-split.md) has no [graph cycle](cycle-in-a-graph.md), so it is a [minimum spanning tree](minimum-spanning-tree.md).

## ↑ Ancestors (7)

1. [Minimum spanning tree](minimum-spanning-tree.md)
2. [Spanning tree](spanning-tree.md)
3. [Tree (graph theory)](tree-graph-theory.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Minimum spanning tree cycle property](minimum-spanning-tree-cycle-property.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/4/solution.md)
