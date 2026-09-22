# Amortized analysis

↑ **Parent:** [Time complexity](time-complexity.md)

[Amortized analysis](amortized-analysis.md) bounds the total cost of every permitted [sequence](sequence.md) of operations from a specified initial state. An amortized $O(1)$ bound means that some constants $a,b$ satisfy $\sum_{i=1}^m c_i\leq am+b$ for every such [sequence](sequence.md) of length $m$. The cost model and allowed operations are part of the claim; [Big O notation](big-o-notation.md) alone does not specify them.

- A worst-case bound for one operation limits its cost in any reachable state. Summing these separate maxima can overestimate the cost of a whole [sequence](sequence.md) because expensive states may take many cheap operations to rebuild.
- An [amortized analysis](amortized-analysis.md) limits the total over every allowed [sequence](sequence.md), including an unfavourably chosen one. Dividing that bound by the number of operations is a deterministic guarantee about the [sequence](sequence.md).
- A probabilistic average-case analysis bounds an [expected value](expected-value-split.md) under a stated [probability distribution](probability-distribution-split.md) on [inputs](input-computer-science.md). For a [randomized algorithm](randomized-algorithm.md), an [expected value](expected-value-split.md) can instead average over its random choices. Neither interpretation is required by a deterministic [amortized analysis](amortized-analysis.md).

This distinction, and the credit and [potential method](potential-method.md) viewpoints, are developed in [R. Endre Tarjan](robert-tarjan.md)'s 1985 paper [Amortized Computational Complexity](https://epubs.siam.org/doi/10.1137/0606031), sections 1–2, pp. 306–308. The [dynamic array doubling](dynamic-array-doubling.md) example below shows how an expensive operation can pay for itself through the cheap operations that precede it.

**Table of contents**

- [Dynamic array doubling](dynamic-array-doubling.md)
- [Potential method](potential-method.md)
  - [Amortized cost](amortized-cost.md)
- [Aggregate analysis](aggregate-analysis.md)
- [Accounting method](accounting-method.md)

## ↑ Ancestors (6)

1. [Time complexity](time-complexity.md)
2. [Complexity class](complexity-class.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Amortized analysis](amortized-analysis.md)
- [Array (data structure)](array-data-structure.md)
- [Breadth-first search](breadth-first-search.md)
- [Circular buffer operation costs](circular-buffer-operation-costs.md)
- [Dynamic array](dynamic-array.md)
- [FIFO queue](fifo-queue.md)
- [Hash table](hash-table.md)
- [Hash table resizing](hash-table-resizing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/iii/solution.md)
- [Robert Tarjan](robert-tarjan.md)
- [Separate chaining](separate-chaining.md)
- [Two-list functional queue](two-list-functional-queue.md)
- [Union by rank](union-by-rank.md)
- [Union-find operation bounds](union-find-operation-bounds.md)
