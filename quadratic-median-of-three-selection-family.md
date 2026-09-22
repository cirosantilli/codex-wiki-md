# Quadratic median-of-three selection family

↑ **Parent:** [Median-of-three pivot selection](median-of-three-pivot-selection.md)

A distinct-input counterexample for [Quickselect](quickselect.md) that chooses the first/middle/last median, reserves it at the last slot, scans lower values to the front, and finally swaps the pivot into place. Let $A_n$ be the following [permutation](permutation.md) of $0,\ldots,n-1$. For $n<4$, take increasing order. For $n\geq4$, let $B=A_{n-2}+2$ componentwise and $m=\lfloor n/2\rfloor$, then set

$$
A_n(0)=1,\quad A_n(m)=0,\quad A_n(n-1)=B(m-2),\quad A_n(1)=B(n-3),
$$

and put $A_n(j)=B(j-2)$ at every other index $2\leq j\leq n-2$. These assignments use every entry of $B$ once and add zero and one, so they really define a [permutation](permutation.md).

The sampled values are $1,0,B(m-2)$, with the last at least two, so the pivot is one. After the initial pivot swap, the only lower value is the zero at index $m$. Moving it to the front places the displaced $B(m-2)$ at its intended tail position. The final pivot swap moves $B(n-3)$ from index one to the last position. Every other tail entry already has its intended position. Thus the complete partitioned result is exactly $[0,1]$ followed by $B$.

Selecting the maximum consequently repeats the same construction on $n-2$ entries. If $C(n)$ counts only pivot comparisons made by the partition scan, then $C(n)=n-1+C(n-2)$, with $C(1)=0$ and $C(2)=1$. Hence $C(n)=\lfloor n^2/4\rfloor$ and total runtime is $\Theta(n^2)$. For example, $A_6=[1,4,3,0,2,5]$. This disproves a linear worst-case claim even when every value is distinct.

## ↑ Ancestors (6)

1. [Median-of-three pivot selection](median-of-three-pivot-selection.md)
2. [Quickselect](quickselect.md)
3. [Selection algorithm](selection-algorithm.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/2/e/solution.md)
