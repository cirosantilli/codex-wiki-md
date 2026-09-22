<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $P^\mu=\partial\mathcal L/\partial(\partial_\mu h)$ and $Q^{\mu\nu}=\partial\mathcal L/\partial(\partial_\mu\partial_\nu h)$. Define the second coefficient with ordered repeated indices and $Q^{\mu\nu}=Q^{\nu\mu}$, so that

$$
\delta\mathcal L=\mathcal L_h\delta h+P^\mu\partial_\mu\delta h+Q^{\mu\nu}\partial_\mu\partial_\nu\delta h.
$$

This convention avoids double-counting a mixed derivative such as $h_{,12}=h_{,21}$. The first derivative term needs one [integration by parts](../../../../integration-by-parts.md). The second derivative term needs two:

$$
\int_\Omega Q^{\mu\nu}\partial_\mu\partial_\nu\delta h
=\text{boundary terms}+\int_\Omega(\partial_\mu\partial_\nu Q^{\mu\nu})\delta h.
$$

Combining the terms gives

$$
\delta S=\int_\Omega\left[\mathcal L_h-\partial_\mu P^\mu+\partial_\mu\partial_\nu Q^{\mu\nu}\right]\delta h
+\int_{\partial\Omega}n_\mu\left[(P^\mu-\partial_\nu Q^{\mu\nu})\delta h+Q^{\mu\nu}\partial_\nu\delta h\right]d\Sigma.
$$

For compactly supported variations, or fixed $\delta h$ and its first derivatives at the boundary, the last integral vanishes. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) then yields the [Euler-Lagrange field equation with second derivatives](../../../../euler-lagrange-field-equation-with-second-derivatives.md):

$$
\boxed{\frac{\partial\mathcal L}{\partial h}
-\partial_\mu\left[\frac{\partial\mathcal L}{\partial(\partial_\mu h)}\right]
+\partial_\mu\partial_\nu\left[\frac{\partial\mathcal L}{\partial(\partial_\mu\partial_\nu h)}\right]=0.}
$$

The plus sign of the final term comes from the two integrations by parts. In general this gives fourth-order equations, although the order in a particular coordinate depends on which second derivatives occur in the density.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
