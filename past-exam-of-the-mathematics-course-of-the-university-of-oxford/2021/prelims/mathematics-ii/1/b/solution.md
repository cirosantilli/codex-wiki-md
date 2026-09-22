<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the first [sequence](../../../../../../sequence.md), $|a_n|=n^{-3}\to0$. The [squeeze theorem](../../../../../../squeeze-theorem.md) gives $a_n\to0$, and every [subsequence](../../../../../../subsequence.md) of a [convergent sequence](../../../../../../convergent-sequence.md) has the same [limit of a sequence](../../../../../../limit-of-a-sequence.md). Thus its [set](../../../../../../set-split.md) of [subsequential limits](../../../../../../subsequential-limit.md) is $\boxed{\{0\}}$.

For the second [sequence](../../../../../../sequence.md), the four possible [sine](../../../../../../sine.md) values give

$$
b_n=\begin{cases}
1,&n\equiv0,2\pmod4,\\
n,&n\equiv1\pmod4,\\
1/n,&n\equiv3\pmod4.
\end{cases}
$$

The even-indexed [subsequence](../../../../../../subsequence.md) is constantly one, and $b_{4k+3}\to0$, so both zero and one occur as [subsequential limits](../../../../../../subsequential-limit.md). A [convergent subsequence](../../../../../../convergent-subsequence.md) is bounded, so it contains only finitely many terms with $n\equiv1\pmod4$. Of the remaining three residue classes, at least one occurs infinitely often. The corresponding further [subsequence](../../../../../../subsequence.md) has [limit of a sequence](../../../../../../limit-of-a-sequence.md) zero or one; the [subsequence](../../../../../../subsequence.md) rule forces the original [convergent subsequence](../../../../../../convergent-subsequence.md) to have that same [limit of a sequence](../../../../../../limit-of-a-sequence.md). Therefore the exact answer is $\boxed{\{0,1\}}$. Divergence to $+\infty$ along $n\equiv1\pmod4$ is not a finite [subsequential limit](../../../../../../subsequential-limit.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
