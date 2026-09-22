<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First take disjoint supports $X,Y$, the setting in which the displayed [Lieb-Robinson bound](../../../../../../lieb-robinson-bound.md) can hold with an $e^{2kst}-1$ factor. For overlapping supports a nonzero equal-time [commutator](../../../../../../commutator.md) is possible, whereas that factor vanishes at $t=0$.

Iterate the given integral inequality for $C_A(Y,t)$. At time zero, $C_A(Y,0)=0$ if $Y$ misses $X$, and in general $C_A(Y,0)\leq2\|A_X\|$. Define the positive interaction-chain weights

$$
a_n(X,Y)=\sum_{\substack{Z_1\cap Y\ne\varnothing,\ Z_{j+1}\cap Z_j\ne\varnothing\\Z_n\cap X\ne\varnothing}}\prod_{j=1}^n\|h_{Z_j}\|.
$$

The [Lieb-Robinson interaction-chain expansion](../../../../../../lieb-robinson-interaction-chain-expansion.md) gives

$$
C_A(Y,t)\leq2\|A_X\|\sum_{n\geq1}\frac{(2|t|)^n}{n!}a_n(X,Y).
$$

The ordered time integrations produce $|t|^n/n!$. For a finite system the iterative remainder tends to zero, since the total interaction weights are finite and the factorial dominates repeated integrations.

For the [interaction distance](../../../../../../interaction-distance.md) convention counting the fewest interacting hyperedges needed to connect disjoint supports, $a_n=0$ when $n<d(X,Y)$. The per-site interaction bound gives

$$
\sum_{Z_1:Z_1\cap Y\ne\varnothing}\|h_{Z_1}\|\leq|Y|s e^{-\mu},\qquad \sum_{Z_{j+1}:Z_{j+1}\cap Z_j\ne\varnothing}\|h_{Z_{j+1}}\|\leq ks e^{-\mu}.
$$

Dropping the final endpoint restriction consequently bounds $a_n\leq|Y|(ks)^ne^{-\mu n}$. Reversing the chains gives the same estimate with $|X|$. Therefore

$$
a_n\leq\min(|X|,|Y|)(ks)^ne^{-\mu n}\leq\min(|X|,|Y|)(ks)^ne^{-\mu d(X,Y)}.
$$

Multiply by $\|B_Y\|$ and sum the exponential series to obtain

$$
\boxed{\|[A_X(t),B_Y]\|\leq2\|A_X\|\|B_Y\|\min(|X|,|Y|)e^{-\mu d(X,Y)}(e^{2ks|t|}-1).}
$$

For overlapping supports, retain the initial term. A valid general version adds $2\|A_X\|\|B_Y\|\mathbf1_{X\cap Y\ne\varnothing}$ to the right side. A coarser bound with $e^{2ks|t|}$ in place of $e^{2ks|t|}-1$ is also sufficient for later shell estimates, with the conventional support distance zero on overlaps. Thus **the printed bound needs disjoint supports or an equal-time term**. The printed $C(Z,s)$ and $O_Z$ inside a supremum over $O_Y$ are also inconsistent labels; the iteration uses $C_A(Z,\tau)$ and $O_Y$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
