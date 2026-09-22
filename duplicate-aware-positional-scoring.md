# Duplicate-aware positional scoring

↑ **Parent:** [Algorithm](algorithm-split.md)

To score a guess against a fixed-length secret, first reserve every equal-position match. For the remaining positions, consume at most one unused secret occurrence for each cow. This two-stage rule prevents an earlier wrong-position token from using the occurrence needed for a later positional match. The sum of bull and cow counts is the [multiset overlap](multiset-overlap.md) of the two sequences. With only [equality tests](equality-test.md), deletion from a list gives a quadratic-time implementation; token-count maps can improve the allocation step when a suitable key representation is available.

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/3/b/solution.md)
