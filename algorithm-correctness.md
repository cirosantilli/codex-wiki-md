# Algorithm correctness

↑ **Parent:** [Algorithm](algorithm-split.md)

[Partial correctness](partial-correctness.md) means that, if the [algorithm](algorithm-split.md) terminates on a permitted [input](input-computer-science.md), its [output](output-computing.md) meets the [formal specification](formal-specification.md). [Total correctness](total-correctness.md) additionally requires [algorithm termination](algorithm-termination.md) on every permitted [input](input-computer-science.md).

A [precondition](precondition.md) $P$ describes permitted starting circumstances; a [postcondition](postcondition.md) $Q$ describes the required result. [Partial correctness](partial-correctness.md) says that starting with $P$ and finishing implies $Q$. [Total correctness](total-correctness.md) also guarantees finishing. A [loop invariant](loop-invariant.md) supplies the connection between these conditions during repeated steps.[CS 2112 Fall 2019; Loop invariants, Using loop invariants to show code is correct: Establishment, Preservation, Postcondition, and Termination](cs-2112-fall-2019/loop-invariants.md)

Correctness is relative to a [formal specification](formal-specification.md). Returning the first entry of an [array](array-data-structure.md) correctly implements "return the first entry", but fails "return the [maximum](maximum-of-a-subset-of-a-total-order.md)" on $[3,1,4,4,2]$. A fast wrong answer does not acquire [algorithm correctness](algorithm-correctness.md) from its [time complexity](time-complexity.md). Numerical closeness matters only when the [formal specification](formal-specification.md) allows an approximation. [Software testing](software-testing.md) and [test coverage](test-coverage.md) provide evidence about selected executions; they do not by themselves establish [algorithm correctness](algorithm-correctness.md) for every permitted [input](input-computer-science.md).

**Table of contents**

- [Partial correctness](partial-correctness.md)
- [Total correctness](total-correctness.md)
  - [Algorithm termination](algorithm-termination.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Formal verification](formal-verification.md)
  - [Summation loop verification](summation-loop-verification.md)
  - [Formal specification](formal-specification.md)
    - [Precondition](precondition.md)
    - [Postcondition](postcondition.md)
  - [Binary correctness](binary-correctness.md)
- [Functional correctness](functional-correctness.md)
- [Loop invariant](loop-invariant.md)
  - [Loop variant](loop-variant.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Algorithm](algorithm-split.md)
- [Algorithm correctness](algorithm-correctness.md)
- [Binary array sum by recursion](binary-array-sum-by-recursion.md)
- [Binary search tree](binary-search-tree.md)
- [Computer science](computer-science-split.md)
- [Correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md)
- [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
- [Factorial recursion and returning frames](factorial-recursion-and-returning-frames.md)
- [Hash table resizing](hash-table-resizing.md)
- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
- [Linear search correctness](linear-search-correctness.md)
- [Linked list](linked-list.md)
- [Loop invariant](loop-invariant.md)
- [Merge algorithm](merge-algorithm.md)
- [Merge sort](merge-sort.md)
- [seL4 verification scope](sel4-verification-scope.md)
- [Sorting algorithm](sorting-algorithm.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)
- [Strong induction for factorization existence](strong-induction-for-factorization-existence.md)
- [Tombstone in open addressing](tombstone-in-open-addressing.md)
