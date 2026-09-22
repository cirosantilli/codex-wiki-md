<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Borsuk conjecture](../../../../../../borsuk-conjecture.md) asserted that every bounded subset of $\mathbb R^d$ of positive diameter can be partitioned into $d+1$ subsets of strictly smaller diameter. We construct a [Kahn-Kalai counterexample to the Borsuk conjecture](../../../../../../kahn-kalai-counterexample-to-the-borsuk-conjecture.md).

For every $2p$-subset $A$ of $[4p]$, let $v_A\in\{-1,1\}^{4p}$ be $1$ on $A$ and $-1$ outside it, and define

$$
x_A=((v_A)_i(v_A)_j)_{1\leq i<j\leq4p}
\in\mathbb R^d,
\qquad d=\binom{4p}{2}.
$$

Because $x_A=x_{A^c}$, retain one representative of each complementary pair. The resulting set $X$ has $\frac12\binom{4p}{2p}$ points. For $s=|A\cap B|$,

$$
v_A\mathbin\cdot v_B=4(s-p),
$$

and

$$
x_A\mathbin\cdot x_B
=\frac{(v_A\mathbin\cdot v_B)^2-4p}{2}.
$$

All $x_A$ have the same norm, so their distance is largest exactly when this inner product is smallest, namely when $s=p$.

Every smaller-diameter part of $X$ therefore corresponds to a family with no pair having intersection $p$. Part ii bounds such a part by $2\binom{4p}{p-1}$. Any smaller-diameter partition consequently needs at least

$$
\frac{\binom{4p}{2p}}{4\binom{4p}{p-1}}
$$

parts. By [Stirling formula](../../../../../../stirling-formula.md), this ratio grows like $(27/16)^p$ up to a polynomial factor, whereas $d+1=O(p^2)$. For every sufficiently large prime $p$, the required number of parts exceeds $d+1$, disproving the conjecture.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
