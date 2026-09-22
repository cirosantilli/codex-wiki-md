<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [continuous semimartingales](../../../../../../continuous-semimartingale.md) $U,V$, the [semimartingale integration by parts](../../../../../../semimartingale-integration-by-parts.md) formula is

$$
\boxed{U_tV_t=U_0V_0+\int_0^tU_s\,dV_s+\int_0^tV_s\,dU_s+[U,V]_t.}
$$

Indeed each partition increment satisfies

$$
\Delta(UV)=U_{\rm left}\Delta V+V_{\rm left}\Delta U+\Delta U\,\Delta V.
$$

Summing telescopes the left side. The first two sums converge to the [stochastic integrals](../../../../../../stochastic-integral.md) by left-endpoint approximation, and the last sum converges to the [quadratic covariation](../../../../../../quadratic-covariation.md) by polarization of the quadratic-increment formula. All limits are in [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md). Hence the equality holds at every time outside one null set, using continuity. In differential notation it is the [Itô product rule](../../../../../../ito-product-rule.md) $d(UV)=U\,dV+V\,dU+d[U,V]$.

For a vector of continuous semimartingales $X=(X^1,\ldots,X^d)$ and $F\in C^{1,2}$, the multidimensional [Itô formula](../../../../../../ito-s-lemma.md) is

$$
\boxed{\begin{aligned}
F(t,X_t)=F(0,X_0)&+\int_0^t\partial_sF(s,X_s)\,ds
+\sum_i\int_0^t\partial_iF(s,X_s)\,dX_s^i\\
&+\frac12\sum_{i,j}\int_0^t\partial_{ij}F(s,X_s)\,d[X^i,X^j]_s.
\end{aligned}}
$$

One route from the product formula is to apply it repeatedly to powers and products of the coordinates, obtaining this expression for polynomials; polarization identifies the mixed second derivatives. Time is another coordinate of [finite variation](../../../../../../total-variation-of-a-function.md), so it has no quadratic-covariation contribution. Localize to compact ranges, approximate a $C^{1,2}$ function and its indicated derivatives by smooth polynomial approximations, and pass to the limit using stochastic-integral continuity and the variation bounds on the finite-variation terms. Equivalently, second-order Taylor expansion along partitions gives the same limit, with integration by parts accounting for every quadratic term.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
