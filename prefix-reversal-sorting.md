# Prefix reversal sorting

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)

To sort a [permutation](permutation.md) using [prefix reversals](prefix-reversal.md), work backwards through final positions. On an active prefix of length $m$, find its largest value. If it is already at the final position, shorten the active prefix. Otherwise move it to the front with one reversal if necessary, then reverse the entire active prefix to put it last. Already settled suffix positions are untouched.

The settled suffix is a [loop invariant](loop-invariant.md), and active-prefix length decreases to one. This proves reachability of the identity [permutation](permutation.md) in at most $2(n-1)$ nontrivial flips. The construction is a finite upper bound, not a promise of minimum length; [breadth-first search](breadth-first-search.md) can find the minimum for small instances.

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/4/d/solution.md)
