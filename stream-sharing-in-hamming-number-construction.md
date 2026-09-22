# Stream sharing in Hamming-number construction

↑ **Parent:** [Sorted multiplicative closure stream](sorted-multiplicative-closure-stream.md)

The [Hamming number](5-smooth-number.md) stream merges its shared multiples by two, three and five. To emit its first $n$ values, each of the fixed number of mapped streams and merge nodes advances at most $n+O(1)$ positions. With [lazy evaluation](lazy-evaluation.md) that shares each evaluated list cell, this takes $\Theta(n)$ comparisons and fixed-factor multiplications. The statement counts arithmetic operations, rather than bits: the growing exact [integers](integer-split.md) make their bit-operation costs larger. Recomputing independent copies of the recursively defined stream loses this sharing argument.

## ↑ Ancestors (6)

1. [Sorted multiplicative closure stream](sorted-multiplicative-closure-stream.md)
2. [Lazy feedback stream](lazy-feedback-stream.md)
3. [Functional programming](functional-programming.md)
4. [Programming language](programming-language-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/2/d/solution.md)
