# Time complexity

↑ **Parent:** [Complexity class](complexity-class.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Time_complexity)

The time complexity of an [algorithm](algorithm.md) bounds its number of computation steps as a function of its input length.

Specify both the size parameter and the operations counted. For [binary search](binary-search.md), take $n$ to be the number of [array](array-data-structure.md) entries and count a three-way comparison of the target with one entry as one operation. Code using separate equality and less-than tests may perform two primitive tests per inspected entry; this changes a constant factor. The [input](input-computer-science.md) size in bits is a different parameter when entries have variable-length representations.

Worst-case [time complexity](time-complexity.md) maximizes the count over permitted [inputs](input-computer-science.md) of size $n$. An absent target forces $n$ comparisons in [linear search](linear-search.md). For [binary search](binary-search.md), the worst-case count is $\lfloor\log_2 n\rfloor+1$ for $n\geq1$, attained by a target larger than every entry. Both have a best case of one comparison when the first inspected entry matches.

In [Big O notation](big-o-notation.md), the worst-case bounds are $O(n)$ and $O(\log n)$ respectively. Here $T(n)=O(g(n))$ means that fixed constants $C,n_0$ exist with $T(n)\leq Cg(n)$ for all $n\geq n_0$. It is an upper bound, so a logarithmic count is also $O(n)$; the sharper bound communicates its scaling better. The base of the [logarithm](logarithm.md) changes only a constant factor.

For $n=1{,}000{,}000$, [linear search](linear-search.md) can require $1{,}000{,}000$ comparisons, whereas [binary search](binary-search.md) needs at most $20$, since $2^{19}\leq n<2^{20}$. Doubling $n$ adds just one to the worst-case [binary search](binary-search.md) count. These are operation counts, not measured machine runtimes. Translating them into logarithmic execution time assumes constant-cost indexed access, comparison and index arithmetic. Long entries can make comparison expensive; a [linked list](linked-list.md) does not provide constant-cost access to an arbitrary middle index. Building or sorting the [array](array-data-structure.md) is additional work: [merge sort](merge-sort.md) can provide order for many subsequent searches, but its cost belongs in the analysis too.

**Table of contents**

- [Pseudo-polynomial time](pseudo-polynomial-time.md)
- [Amortized analysis](amortized-analysis.md)
- [Polynomial time](polynomial-time.md)
  - [Polynomial-time algorithm](polynomial-time-algorithm.md)
  - [P (complexity)](p-complexity.md)
    - [P-completeness](p-completeness.md)
  - [NP (complexity)](np-complexity.md)
    - [Certificate (complexity)](certificate-complexity.md)

## ↑ Ancestors (5)

1. [Complexity class](complexity-class.md)
2. [Computational complexity theory](computational-complexity-theory.md)
3. [Theoretical computer science](theoretical-computer-science.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (50)

- [Algorithm](algorithm.md)
- [Array (data structure)](array-data-structure.md)
- [Asymptotic analysis](asymptotic-analysis.md)
- [Big O notation](big-o-notation.md)
- [Binary heap](binary-heap.md)
- [Binary search](binary-search.md)
- [Binary search tree](binary-search-tree.md)
- [Bipartite graph](bipartite-graph.md)
- [Bit cost of modular exponentiation](bit-cost-of-modular-exponentiation.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Bounding volume hierarchy traversal](bounding-volume-hierarchy-traversal.md)
- [Breadth-first search](breadth-first-search.md)
- [Cached cell value](cached-cell-value.md)
- [Computer science](computer-science-split.md)
- [Cooley-Tukey FFT algorithm](cooley-tukey-fft-algorithm.md)
- [Counting sort](counting-sort.md)
- [Data structure](data-structure.md)
- [Depth-first search](depth-first-search.md)
- [DFS lowpoint](dfs-lowpoint.md)
- [Dijkstra algorithm](dijkstra-algorithm.md)
- [Dynamic programming](dynamic-programming.md)
- [Fast Fourier transform](fast-fourier-transform.md)
- [FIFO queue](fifo-queue.md)
- [Hash table](hash-table.md)
- [Insertion sort](insertion-sort.md)
- [Kahn's algorithm](kahn-s-algorithm.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
- [Linked list](linked-list.md)
- [Longest increasing subsequence](longest-increasing-subsequence.md)
- [Memoization arithmetic and stack costs](memoization-arithmetic-and-stack-costs.md)
- [Merge algorithm](merge-algorithm.md)
- [Merge sort](merge-sort.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/9/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/9/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120/1/e/solution.md)
- [Prefix sum](prefix-sum.md)
- [Radix sort](radix-sort.md)
- [Representation independence](representation-independence.md)
- [Separate chaining](separate-chaining.md)
- [Sorted array](sorted-array.md)
- [Time complexity](time-complexity.md)
