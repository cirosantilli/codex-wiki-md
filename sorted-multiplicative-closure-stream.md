# Sorted multiplicative closure stream

↑ **Parent:** [Lazy feedback stream](lazy-feedback-stream.md)

For a finite nonempty collection of exact real multipliers greater than one, the multiplicative closure of one can be enumerated by a shared [lazy list](lazy-list.md): emit one, then merge its elementwise multiples by all generators. Every value after one has a smaller predecessor obtained by removing one factor, proving [productivity](stream-productivity.md) by increasing value. There are only finitely many exponent tuples below any fixed bound, because every generator is greater than one; thus [locally finite sorted-stream merge](locally-finite-sorted-stream-merge.md) eventually emits every generated value. Equal products are emitted once.

A multiplier below one contradicts increasing order starting at one. A multiplier equal to one adds no new values and should be removed from the recursive streams; an empty remaining generator collection has the finite closure consisting of one. These qualifications concern exact arithmetic: finite precision or overflow can violate the order and growth assumptions.

**Table of contents**

- [Stream sharing in Hamming-number construction](stream-sharing-in-hamming-number-construction.md)

## ↑ Ancestors (5)

1. [Lazy feedback stream](lazy-feedback-stream.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/2/e/solution.md)
