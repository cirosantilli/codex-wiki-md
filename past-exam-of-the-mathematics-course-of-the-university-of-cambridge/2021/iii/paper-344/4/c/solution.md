<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\tau=|t-t'|$. Integrating the equation for $x$ and using independence of the two noises gives

$$
R(\tau)
=C^2\tau+
\int_0^\tau\int_0^\tau
f_0^2e^{-\alpha|s-s'|}\,ds\,ds'.
$$

With the supplied integral,

$$
\boxed{
R(\tau)
=C^2\tau+
\frac{2f_0^2}{\alpha^2}
\left(\alpha\tau-1+e^{-\alpha\tau}\right)
}.
$$

For $\alpha\tau\ll1$, the active contribution is ballistic, $f_0^2\tau^2+O(\tau^3)$, in addition to the Brownian term. For $\alpha\tau\gg1$,

$$
R(\tau)
=\left(C^2+\frac{2f_0^2}{\alpha}\right)\tau
-\frac{2f_0^2}{\alpha^2}+o(1),
$$

so the long-time motion is diffusive with an enhanced [diffusion coefficient](../../../../../../diffusion-coefficient.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
