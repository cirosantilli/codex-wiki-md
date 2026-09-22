<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $E=\mathbb R[x]_{\le d}$ with the [supremum norm](../../../../../../supremum-norm.md). By [equivalence of norms in finite dimensions](../../../../../../equivalence-of-norms-in-finite-dimensions.md), there is $C_d$ such that $\sum_{j=0}^d|a_j|\le C_d\|p\|_\infty$ whenever $p=\sum_j a_jx^j$. Hence

$$
\|(B_n-I)p\|_\infty\le\sum_j|a_j|\|B_n(x^j)-x^j\|_\infty,
$$

so $\varepsilon_n:=\|B_n-I\|_{\rm op}\le C_d\max_{0\le j\le d}\|B_n(x^j)-x^j\|_\infty\to0$. This upgrades convergence on fixed polynomials to [operator norm](../../../../../../operator-norm.md) convergence on the fixed space.

For sufficiently large $n$, $\varepsilon_n<1$, and a [Neumann series](../../../../../../neumann-series.md) gives

$$
\|B_n^{-1}-I\|_{\rm op}\le\frac{\varepsilon_n}{1-\varepsilon_n}.
$$

Thus the [inverse Bernstein approximation on a fixed-degree polynomial space](../../../../../../inverse-bernstein-approximation-on-a-fixed-degree-polynomial-space.md) satisfies $\|g_n-f\|_\infty\to0$. By the [extreme value theorem](../../../../../../extreme-value-theorem.md), strict positivity on the compact interval gives $\mu=\min_{[0,1]}f>0$. Eventually $\|g_n-f\|_\infty<\mu/2$, and consequently

$$
\boxed{g_n(x)\ge\mu/2>0\quad\text{on }[0,1]\text{ for all sufficiently large }n.}
$$

Applying pointwise convergence to the varying polynomials $g_n$ without this finite-dimensional operator argument would not justify the conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
