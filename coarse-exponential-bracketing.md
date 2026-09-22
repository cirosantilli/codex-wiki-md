# Coarse exponential bracketing

↑ **Parent:** [Exponential search](exponential-search.md)

To discover a positive unknown [integer](integer-split.md) $m$ by comparisons, test the thresholds $2^k,2^{2k},\ldots$ for fixed $k\ge1$. If the first threshold not smaller than $m$ has index $j$, fewer than $2^{kj}$ candidates remain and [binary search](binary-search.md) needs at most $kj+O(1)$ comparisons. Since $j\le\log_2(m)/k+1$, the total is at most $(1+1/k)\log_2 m+O_k(1)$. Choosing $k\ge1/\epsilon$ makes the leading constant at most $1+\epsilon$; the additive constant may depend on $\epsilon$.

## ↑ Ancestors (4)

1. [Exponential search](exponential-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/5/b/solution.md)
