<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

The real [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) says that a subalgebra of $C(X,\mathbb R)$ on a compact metric space is uniformly dense if it contains the constants and separates points. The finite sums $\sum_i f_i(x)g_i(y)$ form such an algebra on $[0,1]^2$: multiplication preserves this form, the constant one belongs to it, and the coordinate functions distinguish every pair of different points. Thus they approximate the continuous kernel uniformly.

A [finite-rank operator](../../../../../finite-rank-operator.md) has finite-dimensional range. A [compact operator](../../../../../compact-operator-split.md) maps the unit ball to a set with compact closure, equivalently sends every bounded sequence to a sequence with a convergent subsequence. The identity on $C[0,1]$ is bounded but not compact: the functions $x^n$ have supremum norm one, and every subsequence has the discontinuous pointwise limit which is zero on $[0,1)$ and one at one. It therefore has no uniformly convergent subsequence.

A bounded finite-rank operator is compact because bounded sets in its finite-dimensional range have compact closure. Suppose $T_n\to T$ in [operator norm](../../../../../operator-norm.md). For any $\varepsilon>0$, choose $n$ with $\|T-T_n\|<\varepsilon/3$ and a finite $\varepsilon/3$-net for $T_n$ of the unit ball. The same centres give an $\varepsilon$-net for $T$ of that ball. Its closure is totally bounded and complete in the [Banach space](../../../../../banach-space-split.md) $Y$, hence compact. Thus **an operator-norm limit of compact operators is compact**.

For $K_n(x,y)=\sum_i f_i(x)g_i(y)$ uniformly approximating $K$, the integral operator $T_n$ has range in $\operatorname{span}\{f_i\}$ and is bounded. Moreover

$$
\|(T-T_n)f\|_\infty\leq\|K-K_n\|_\infty\|f\|_\infty.
$$

Consequently $T_n\to T$ in operator norm, proving that **the stated integral operator is compact**.

## ↑ Ancestors (11)

1. [22G](../22g.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
