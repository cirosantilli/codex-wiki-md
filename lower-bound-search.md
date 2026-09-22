# Lower-bound search

↑ **Parent:** [Binary search](binary-search.md)

For a nondecreasing [sorted array](sorted-array.md) $a[0..N)$ and target $x$, find the unique position $p\in[0,N]$ such that every earlier value is below $x$ and every later value is at least $x$. Equivalently, $p=\min(\{i\in[0,N):a(i)\geq x\}\cup\{N\})$. Uniqueness follows because, if $p<q$ both satisfied the partition, $a(p)$ would have to be both at least $x$ and below $x$. A half-open search interval maintains an excluded prefix of smaller values and an excluded suffix of greater-or-equal values. Allowing the sentinel $N$ handles an empty array or a target beyond its last entry.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Distinct-index two-sum by suffix lower bounds](distinct-index-two-sum-by-suffix-lower-bounds.md)
- [Equal-range search](equal-range-search.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/1/d/solution.md)
- [Ternary lower-bound search](ternary-lower-bound-search.md)
