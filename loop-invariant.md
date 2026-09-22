# Loop invariant

↑ **Parent:** [Algorithm correctness](algorithm-correctness.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_invariant)

A statement true whenever execution reaches a chosen point in a loop, usually immediately before its condition is tested. Establish it initially, preserve it through each iteration, and combine it with the exit condition to establish [algorithm correctness](algorithm-correctness.md). Termination needs a separate argument.[CS 2112 Fall 2019; Loop invariants, Using loop invariants to show code is correct: the three partial-correctness obligations and separate Termination step](cs-2112-fall-2019/loop-invariants.md)

Write $I$ for the [loop invariant](loop-invariant.md), $B$ for the condition, $P$ for the [precondition](precondition.md), and $Q$ for the [postcondition](postcondition.md). Prove that initialization under $P$ establishes $I$, that a completed body starting with $I$ and $B$ restores $I$, and that $I$ with false $B$ implies $Q$.[CS 2112 Fall 2019; Loop invariants, Using loop invariants to show code is correct: Establishment, Preservation, and Postcondition](cs-2112-fall-2019/loop-invariants.md)

In the [prefix maximum correctness example](prefix-maximum-correctness-example.md), the [loop invariant](loop-invariant.md) remembers exactly the [maximum](maximum-of-a-subset-of-a-total-order.md) of the processed prefix and the valid index bounds. The weaker statement $\mathrm{best}\geq a_0$ survives every iteration, but does not imply the [postcondition](postcondition.md): for $[3,1,4,4,2]$, the wrong value $3$ satisfies it. A useful [loop invariant](loop-invariant.md) retains enough information to recover the answer when the condition becomes false.

**Table of contents**

- [Loop variant](loop-variant.md)

## ↑ Ancestors (4)

1. [Algorithm correctness](algorithm-correctness.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Algorithm](algorithm-split.md)
- [Algorithm correctness](algorithm-correctness.md)
- [Binary search](binary-search.md)
- [Conditional expectation choice invariant](conditional-expectation-choice-invariant.md)
- [Exponentiation by squaring](exponentiation-by-squaring.md)
- [Formal verification](formal-verification.md)
- [Greedy-choice property](greedy-choice-property.md)
- [Insertion sort](insertion-sort.md)
- [Kruskal safe edge](kruskal-safe-edge.md)
- [Linear search correctness](linear-search-correctness.md)
- [Loop invariant](loop-invariant.md)
- [Loop variant](loop-variant.md)
- [Mathematical induction](mathematical-induction.md)
- [Merge algorithm](merge-algorithm.md)
- [Modular exponentiation](modular-exponentiation.md)
- [Partial correctness](partial-correctness.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Radix sort suffix invariant](radix-sort-suffix-invariant.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)
- [Summation loop verification](summation-loop-verification.md)
- [Tentative distance](tentative-distance.md)
- [Total correctness](total-correctness.md)
