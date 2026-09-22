# Sortedness

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)

For an [output](output-computing.md) [sequence](sequence.md) $B$ of length $n$, [sortedness](sortedness.md) means

$$
k(B_i)\leq k(B_{i+1})\qquad(0\leq i<n-1)
$$

under the chosen [total order](total-order.md) on [sort keys](sort-key.md). Its [transitivity](transitive-relation.md) also gives $k(B_i)\leq k(B_j)$ whenever $i<j$. An empty [sequence](sequence.md) and a one-entry [sequence](sequence.md) satisfy [sortedness](sortedness.md) without any adjacent comparison. For longer [sequences](sequence.md), checking adjacent pairs suffices; checking only the first and last [sort keys](sort-key.md) does not. For example, $(1,3,2,4)$ passes an endpoint comparison but fails [sortedness](sortedness.md) at $3,2$. [Sortedness](sortedness.md) alone says nothing about which [input](input-computer-science.md) entries survived.

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Insertion sort](insertion-sort.md)
- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/4/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/4/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/1/c/solution.md)
- [Radix sort suffix invariant](radix-sort-suffix-invariant.md)
- [Sortedness](sortedness.md)
- [Sorting algorithm](sorting-algorithm.md)
- [Stable digit sort](stable-digit-sort.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)
- [Ternary lower-bound search](ternary-lower-bound-search.md)
- [Upper-bound search](upper-bound-search.md)
