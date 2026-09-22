# Lazy feedback stream

↑ **Parent:** [Functional programming](functional-programming.md)

Mutually dependent streams evaluated by [lazy evaluation](lazy-evaluation.md). A useful sufficient condition for [productivity](stream-productivity.md) is that one participant emits its first constructor independently of any reply, while its $(j+1)$-st output depends only on the first $j$ replies. A scorer mapping each guess to a terminating response then lets each finite interaction prefix be constructed inductively. Inspecting the reply stream before emitting the first guess instead creates a circular demand.

**Table of contents**

- [Sorted multiplicative closure stream](sorted-multiplicative-closure-stream.md)
  - [Stream sharing in Hamming-number construction](stream-sharing-in-hamming-number-construction.md)

## ↑ Ancestors (4)

1. [Functional programming](functional-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Lazy evaluation](lazy-evaluation.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/3/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/3/d/solution.md)
