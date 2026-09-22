# Sorted array

↑ **Parent:** [Array (data structure)](array-data-structure.md)

An [array](array-data-structure.md) whose entries appear in nondecreasing order under a specified [total order](total-order.md). The displayed inequalities allow repeated values.

For example, $(2,5,5,9)$ is a [sorted array](sorted-array.md) of [integers](integer-split.md). Inserting $7$ at index $3$ gives $(2,5,5,7,9)$: with spare capacity, first shift $9$ one slot right. Appending $7$ would violate the [sorted array](sorted-array.md) property. Updating an entry also requires preserving the [total order](total-order.md), or removing and reinserting it in a suitable position.

The useful combination is order plus direct indexed access: [binary search](binary-search.md) eliminates a whole interval of candidates at each comparison, giving $O(\log n)$ search [time complexity](time-complexity.md) under constant-cost comparisons and the [array](array-data-structure.md) cost model. A [sorted array](sorted-array.md) is therefore attractive for many lookups between changes, while keeping it sorted can still require $O(n)$ shifting work per insertion. A sorted [linked list](linked-list.md) has the ordering information but does not supply the same constant-cost access to a middle index.

## ↑ Ancestors (4)

1. [Array (data structure)](array-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Adjacency list storage and query costs](adjacency-list-storage-and-query-costs.md)
- [Algorithm](algorithm-split.md)
- [Binary heap](binary-heap.md)
- [Binary search](binary-search.md)
- [Computer science](computer-science-split.md)
- [Data structure](data-structure-split.md)
- [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
- [Heap order](heap-order.md)
- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
- [Linear search](linear-search.md)
- [Merge sort](merge-sort.md)
- [Priority queue](priority-queue.md)
- [Sorted array](sorted-array.md)
- [Sorting algorithm](sorting-algorithm.md)
