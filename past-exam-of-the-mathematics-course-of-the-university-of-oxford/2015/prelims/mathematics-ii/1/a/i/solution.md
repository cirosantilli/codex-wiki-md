<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Call $k$ a [peak of a sequence](../../../../../../../peak-of-a-sequence.md) when $a_k\geq a_m$ for every $m>k$. If there are infinitely many [peaks of a sequence](../../../../../../../peak-of-a-sequence.md), list their indices in increasing order, $k_1<k_2<\cdots$. Since $k_{r+1}>k_r$,

$$
\boxed{a_{k_1}\geq a_{k_2}\geq\cdots.}
$$

This is a decreasing [subsequence](../../../../../../../subsequence.md); throughout this argument, a decreasing [monotone sequence](../../../../../../../monotone-sequence.md) may have equal successive terms.

If there are only finitely many [peaks of a sequence](../../../../../../../peak-of-a-sequence.md), choose $N$ beyond all their indices; take $N=1$ if there are none. Every $n\geq N$ fails to be a [peak of a sequence](../../../../../../../peak-of-a-sequence.md), so some $m>n$ satisfies $a_m>a_n$. Starting with $n_1=N$, choose such an $n_{r+1}>n_r$ recursively. This gives

$$
\boxed{a_{n_1}<a_{n_2}<\cdots.}
$$

The two cases prove the [monotone subsequence theorem](../../../../../../../monotone-subsequence-theorem.md) without any boundedness hypothesis.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
