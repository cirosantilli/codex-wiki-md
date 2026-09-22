<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Differentiate the bound with respect to one $J(q)$, using $\partial S_0/\partial J(q)=-J(q)^{-2}$ and $\partial S_2/\partial J(q)=-q^2J(q)^{-2}$:

$$
0=\frac1{J(q)}-\frac{G(q)}{J(q)^2}-\frac{4B}{VJ(q)^2}(S_2+q^2S_0).
$$

Thus an interior minimizing [Gaussian variational kernel for a gradient quartic interaction](../../../../../../gaussian-variational-kernel-for-a-gradient-quartic-interaction.md) has

$$
\boxed{J(q)=\bar a+\bar\kappa q^2+\gamma q^4,\qquad
\bar a=a+\frac{4B}{V}S_2,\quad\bar\kappa=\kappa+\frac{4B}{V}S_0.}
$$

Use the half-space mode density given in the question. In the [thermodynamic limit](../../../../../../thermodynamic-limit.md), the coupled [self-consistency equations](../../../../../../self-consistency-equation.md) are

$$
\boxed{\begin{aligned}
\bar a&=a+2B\int_{|k|<\Lambda}\frac{k^2}{\bar a+\bar\kappa k^2+\gamma k^4}\frac{d^dk}{(2\pi)^d},\\
\bar\kappa&=\kappa+2B\int_{|k|<\Lambda}\frac1{\bar a+\bar\kappa k^2+\gamma k^4}\frac{d^dk}{(2\pi)^d}.
\end{aligned}}
$$

The admissible solution must have $J(q)>0$. The coefficient $\gamma$ is unchanged because the interaction's derivative contributes only a constant and a $q^2$ term.

The formal continuum integrals require the coarse-graining [ultraviolet cutoff](../../../../../../ultraviolet-cutoff.md) $\Lambda$ in three dimensions: the first radial integrand tends to a constant at large $k$, so taking $\Lambda=\infty$ would leave $\bar a$ divergent. The low-wavevector fluctuation argument is independent of this short-distance regularization.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
