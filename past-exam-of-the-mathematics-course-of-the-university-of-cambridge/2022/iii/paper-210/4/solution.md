<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [pushforward measure](../../../../../pushforward-measure.md) of $\mu$ under $g$ is

$$
(g_*\mu)(B)=\mu(g^{-1}(B)),
\qquad B\in\mathcal B.
$$

The [Lebesgue decomposition theorem](../../../../../lebesgue-decomposition-theorem.md) says that for sigma-finite measures $P,Q$ there are unique measures $P_{\rm ac}$ and $P_{\rm s}$ such that

$$
P=P_{\rm ac}+P_{\rm s},
\qquad
P_{\rm ac}\ll Q,
\qquad
P_{\rm s}\perp Q.
$$

For a convex lower-semicontinuous function $f$ with $f(1)=0$, choose any measure $\lambda$ dominating probability measures $P,Q$, put $p=dP/d\lambda$ and $q=dQ/d\lambda$, and define the [f-divergence](../../../../../f-divergence.md)

$$
D_f(P\Vert Q)=\int q f(p/q)\,d\lambda,
$$

using the lower-semicontinuous perspective value when $q=0$. This definition includes the singular part and is independent of $\lambda$.

To prove the [data processing inequality for f-divergences](../../../../../data-processing-inequality-for-f-divergences.md), let $\mathcal G=\sigma(g)$ and use $\lambda=P+Q$. The densities of $g_*P$ and $g_*Q$, pulled back to $\mathcal G$, are $\mathbb E_\lambda(p\mid\mathcal G)$ and $\mathbb E_\lambda(q\mid\mathcal G)$. Since the perspective

$$
\Phi(a,b)=bf(a/b)
$$

is jointly convex, conditional [Jensen inequality](../../../../../jensen-s-inequality.md) gives

$$
\Phi\{\mathbb E(p\mid\mathcal G),\mathbb E(q\mid\mathcal G)\}
\leq\mathbb E\{\Phi(p,q)\mid\mathcal G\}.
$$

Integration proves

$$
D_f(g_*P\Vert g_*Q)\leq D_f(P\Vert Q).
$$

The [chi-squared divergence](../../../../../chi-squared-divergence.md) is

$$
\chi^2(P,Q)
=\int\left(\frac{dP}{dQ}-1\right)^2dQ
$$

when $P\ll Q$, and is infinite otherwise.

Fix a probability measure $Q$. Let $J$ be uniform on $\{1,\ldots,M\}$ and, conditionally on $J=j$, draw $X$ from $P_j$. Compare this joint law with the reference law under which $J$ is uniform and independent of $X\sim Q$. For

$$
H(J,X)=\mathbf1_{\{X\in A_J\}},
$$

the target expectation is $M^{-1}\sum_jP_j(A_j)$, while its reference expectation is

$$
\frac1M\sum_jQ(A_j)=\frac1M
$$

because the $A_j$ form a partition. Its reference variance is $M^{-1}(1-M^{-1})$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) applied to the likelihood ratio gives

$$
\frac1M\sum_jP_j(A_j)-\frac1M
\leq
\sqrt{\frac1M\left(1-\frac1M\right)}
\sqrt{\chi^2(P_{J,X},U_M\otimes Q)}.
$$

The last divergence separates over $J$:

$$
\chi^2(P_{J,X},U_M\otimes Q)
=\frac1M\sum_{j=1}^M\chi^2(P_j,Q).
$$

Taking the infimum over all probability measures $Q$ proves the required inequality.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
