<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\alpha=a/q+\beta$, where $|\beta|\leq q^{-2}$. Split the $m$-interval into $O(M/q+1)$ consecutive blocks of length at most $q/2$. If distinct integers $m,n$ lie in one block, then $0<|m-n|<q/2$. Since $(a,q)=1$,

$$
\left\|\frac{a(m-n)}q\right\|\geq\frac1q,
$$

whereas $|\beta(m-n)|\leq1/(2q)$. Hence $\|\alpha m-\alpha n\|\geq1/(2q)$.

The points $\alpha m$ in one block are therefore $1/(2q)$-separated modulo one. Order them by distance from the nearest integer. Apart from a bounded number of endpoints, the $j$th closest point has distance $\gg j/q$, and consequently

$$
\sum_{m\text{ in one block}}\min(R,\|\alpha m\|^{-1})
\ll R+q\sum_{1\leq j\leq q}\frac1j
\ll R+q\log q.
$$

Multiplying by $O(M/q+1)$ gives

$$
\boxed{
\sum_{m_0\leq m<m_0+M}\min(R,\|\alpha m\|^{-1})
\ll(\log q)\left(\frac{MR}{q}+M+R+q\right).}
$$

This is the [reciprocal fractional-part sum near a rational](../../../../../../reciprocal-fractional-part-sum-near-a-rational.md) estimate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
