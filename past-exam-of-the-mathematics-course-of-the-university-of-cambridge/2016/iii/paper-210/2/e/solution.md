<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Two independent cyclic intervals intersect with [probability](../../../../../../probability.md) at most $\min\{1,(2k-1)/d\}\leq2k/d$. For $k\leq d/2$, precisely the $2k-1$ starting-point offsets $-(k-1),\ldots,k-1$ can overlap; for larger $k$, the upper bound is automatic. The [cyclic interval overlap bound](../../../../../../cyclic-interval-overlap-bound.md) and the preceding [chi-squared divergence](../../../../../../chi-squared-divergence.md) estimate therefore give

$$
\chi^2(P_{\theta,n}\Vert P_0^{\otimes n})\leq\frac{2k}{d}(e^{n\theta^2}-1)\leq2d^{-\varepsilon}(\alpha d)^\varepsilon=2\alpha^\varepsilon.
$$

As in 1(e), the square-root hypothesis is meaningful when $\alpha d\geq1$. The [chi-squared testing lower bound](../../../../../../chi-squared-testing-lower-bound.md) bounds the [total variation distance](../../../../../../total-variation-distance.md) by $\sqrt{2\alpha^\varepsilon}/2$. The worst individual [Type II error](../../../../../../type-i-and-type-ii-errors.md) dominates the error under the uniform [mixture model](../../../../../../mixture-model.md). Thus

$$
\boxed{\inf_\psi\max\{P_0^{\otimes n}(\psi=1),\max_{S\in\mathcal S}P_{\theta,S}^{\otimes n}(\psi=0)\}\geq\tfrac12-\nu_{\varepsilon,\alpha},\quad\nu_{\varepsilon,\alpha}=\frac{\sqrt{2\alpha^\varepsilon}}4.}
$$

Taking $\alpha$ small makes this lower bound informative. This argument uses the actual cyclic-interval alternative, without substituting a different family of subsets.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
