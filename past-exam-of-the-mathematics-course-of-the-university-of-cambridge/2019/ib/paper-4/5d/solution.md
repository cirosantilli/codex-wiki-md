<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

Introduce the [Cauchy approximate identity](../../../../../cauchy-approximate-identity.md)

$$
\delta_\varepsilon(x)=\frac{\varepsilon}{\pi(\varepsilon^2+x^2)}.
$$

It is an [approximate identity](../../../../../approximate-identity.md) converging to the [Dirac delta function](../../../../../dirac-delta-function.md) $\delta$, and $g_\varepsilon=\delta_\varepsilon'$. For a smooth rapidly decaying [test function](../../../../../test-function.md) $\phi$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\int_{-\infty}^{\infty}\phi(x)g_\varepsilon(x)\,dx
=-\int_{-\infty}^{\infty}\phi'(x)\delta_\varepsilon(x)\,dx
\longrightarrow-\phi'(0).
$$

By the definition of the [derivative of the Dirac delta](../../../../../derivative-of-the-dirac-delta.md), $\langle\delta',\phi\rangle=-\phi'(0)$. Therefore the limit as a [distribution](../../../../../distribution-mathematical-analysis.md) is

$$
\boxed{g_\varepsilon\longrightarrow\delta'}.
$$

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
