# Two-sorted-array order statistic

↑ **Parent:** [Selection algorithm](selection-algorithm.md)

To obtain the $k$-th smallest entry of two ascending [sorted arrays](sorted-array.md) of lengths $m,n$, choose prefix lengths $i,j$ with $i+j=k$. Search $\max(0,k-n)\le i\le\min(m,k)$ for the two boundary inequalities in the title, treating missing left boundaries as $-\infty$ and missing right boundaries as $+\infty$. Then all $k$ selected entries precede all unselected entries, so their largest boundary value is the answer. If $A_L>B_R$, decrease $i$; if $B_L>A_R$, increase $i$. These failures are monotone because one prefix grows as the other shrinks. [Binary search](binary-search.md) thus takes $O(\log(\min(m,n)+1))$ comparisons when the shorter [array](array-data-structure.md) supplies the searched prefix. Repeated values retain their multiplicities in the ranks.

## ↑ Ancestors (4)

1. [Selection algorithm](selection-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/5/c/solution.md)
