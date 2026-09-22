<h1 id="7e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For finite [sets](../../../../../../set-split.md) $C_1,\ldots,C_k$, the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) states

$$
\boxed{\left|\bigcup_{j=1}^kC_j\right|
=\sum_{\varnothing\ne J\subseteq[k]}(-1)^{|J|+1}
\left|\bigcap_{j\in J}C_j\right|.}
$$

In a finite ambient [set](../../../../../../set-split.md) $\Omega$, its equivalent complement form is

$$
\left|\Omega\setminus\bigcup_{j=1}^kC_j\right|
=\sum_{J\subseteq[k]}(-1)^{|J|}
\left|\bigcap_{j\in J}C_j\right|,
$$

where the intersection for $J=\varnothing$ means $\Omega$. To see the counting mechanism, an element in exactly $r\ge1$ of the [sets](../../../../../../set-split.md) has coefficient $\sum_{i=1}^r(-1)^{i+1}\binom ri=1$, by the [binomial theorem](../../../../../../binomial-theorem.md); an element in none has coefficient zero in the union formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7E](../../7e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
