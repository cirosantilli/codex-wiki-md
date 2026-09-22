<h1 id="6e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) states that for finite sets $A_1,\ldots,A_k$,

$$
\left|\bigcup_iA_i\right|
=\sum_i|A_i|-\sum_{i<j}|A_i\cap A_j|+\cdots+(-1)^{k+1}|A_1\cap\cdots\cap A_k|.
$$

For each prime $p\mid n$, exclude pairs whose two coordinates are divisible by $p$. For a set of distinct prime divisors $p_1,\ldots,p_j$, exactly $n^2/(p_1\cdots p_j)^2$ pairs have both coordinates divisible by their product. Inclusion-exclusion therefore gives

$$
\boxed{|Y|=n^2\prod_{p\mid n}\left(1-\frac1{p^2}\right)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
