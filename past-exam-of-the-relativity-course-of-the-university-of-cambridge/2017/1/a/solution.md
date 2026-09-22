<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Christoffel symbol](../../../../christoffel-symbol.md) formula with its first index raised:

$$
\Gamma^i{}_{jk}=\frac12g^{i\ell}(\partial_jg_{\ell k}+\partial_kg_{\ell j}-\partial_\ell g_{jk}).
$$

The diagonal [metric tensor](../../../../metric-tensor.md) has $g_{rr}=e^{2\chi}$ and $g_{\theta\theta}=r^2e^{2\chi}$, with inverse components $g^{rr}=e^{-2\chi}$ and $g^{\theta\theta}=r^{-2}e^{-2\chi}$. Since $\partial_r\chi=\chi'$ and all angular derivatives vanish,

$$
\boxed{\Gamma^r{}_{rr}=\chi',\qquad
\Gamma^r{}_{\theta\theta}=-r-r^2\chi',\qquad
\Gamma^\theta{}_{\theta r}=\Gamma^\theta{}_{r\theta}=\frac1r+\chi'.}
$$

For example, $\Gamma^r{}_{\theta\theta}=-\tfrac12e^{-2\chi}\partial_r(r^2e^{2\chi})$. The other components vanish. The formula supplied in the paper gives the first-kind coefficients $\Gamma_{ijk}$; multiplication by the inverse [metric tensor](../../../../metric-tensor.md) is needed for the requested second-kind coefficients. These [polar coordinates](../../../../polar-coordinates.md) are understood away from $r=0$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
