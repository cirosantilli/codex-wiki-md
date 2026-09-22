# FIFO queue

↑ **Parent:** [Data structure](data-structure.md)

A [FIFO queue](fifo-queue.md) is a [data structure](data-structure.md) with first-in, first-out behavior: `enqueue` inserts at the rear, `dequeue` removes and returns the front, and `peek` inspects the front without removing it. Removal and inspection require a nonempty [FIFO queue](fifo-queue.md), or an explicitly defined empty-case result. Enqueue $A,B,C$ in that order, dequeue $A$, then enqueue $D$: the remaining [sequence](sequence.md) is $B,C,D$, with $B$ next. A [LIFO stack](stack-data-structure.md) would remove the most recently inserted item instead. A [FIFO queue](fifo-queue.md) models arrival-order service and supplies the next [vertex](vertex-graph-theory.md) for [breadth-first search](breadth-first-search.md); a stochastic service model belongs to [queueing theory](queueing-theory-split.md). [Sedgewick and Wayne, Algorithms: Queue interface and implementation](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/Queue.java)

The [FIFO queue](fifo-queue.md) interface specifies removal order, not [time complexity](time-complexity.md). A [linked list](linked-list.md) with both front and rear pointers supports `enqueue`, `dequeue` and `peek` in $O(1)$ worst-case time under constant-cost pointer operations and allocation, as in Sedgewick and Wayne's implementation. A plain [array](array-data-structure.md) that deletes its first entry by shifting the remaining $n-1$ entries takes $O(n)$ time per such removal. An [array](array-data-structure.md) with advancing front and rear indices can avoid these shifts; storage and resizing policies still need analysis. The [two-list functional queue](two-list-functional-queue.md) gives a different implementation with constant [amortized analysis](amortized-analysis.md) cost along a single sequence of uses. These representation choices matter when deriving the linear [time complexity](time-complexity.md) of [breadth-first search](breadth-first-search.md) in [Big O notation](big-o-notation.md).

// Destination: computer-science.bigb

**Table of contents**

- [Two-list functional queue](two-list-functional-queue.md)

## ↑ Ancestors (3)

1. [Data structure](data-structure.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Abstract data type](abstract-data-type.md)
- [Application programming interface](application-programming-interface.md)
- [Bipartite graph](bipartite-graph.md)
- [Bounded queue with encapsulation](bounded-queue-with-encapsulation.md)
- [Breadth-first search](breadth-first-search.md)
- [Circular buffer](circular-buffer.md)
- [Data structure](data-structure.md)
- [FIFO page replacement](fifo-page-replacement.md)
- [FIFO queue](fifo-queue.md)
- [Information hiding](information-hiding.md)
- [Kahn's algorithm](kahn-s-algorithm.md)
- [Linked list](linked-list.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/iii/solution.md)
- [Ready queue](ready-queue.md)
- [Representation exposure](representation-exposure.md)
- [Round-robin scheduling](round-robin-scheduling.md)
- [Stack (data structure)](stack-data-structure.md)
