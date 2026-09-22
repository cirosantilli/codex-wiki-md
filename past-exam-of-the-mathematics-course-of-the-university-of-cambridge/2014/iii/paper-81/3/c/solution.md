<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In sector $m$, separate the stationary winding path from its endpoint-fixed fluctuations:

$$
\phi(\tau)=\phi_0+\frac{2\pi m}{\beta}\tau+\eta(\tau),\qquad\eta(0)=\eta(\beta)=0.
$$

The cross term integrates to $2(2\pi m/\beta)[\eta(\beta)-\eta(0)]=0$. Hence

$$
\frac{I}{2\hbar^2}\int_0^\beta\dot\phi^2d\tau
=\frac{I(2\pi m)^2}{2\hbar^2\beta}+\frac{I}{2\hbar^2}\int_0^\beta\dot\eta^2d\tau.
$$

The Gaussian fluctuation integral is independent of $m$ and $\phi_0$. Denoting it by $\mathcal Z_0$, integration over the starting angle gives

$$
\boxed{\mathcal Z=2\pi\mathcal Z_0\sum_{m\in\mathbb Z}e^{-I(2\pi m)^2/(2\hbar^2\beta)}.}
$$

The [rotor return-kernel fluctuation prefactor](../../../../../../rotor-return-kernel-fluctuation-prefactor.md) $\mathcal Z_0$ is the coincident-point free-particle kernel on the lifted line, or the return amplitude density from zero-net-winding paths. It is not the $n=0$ angular-momentum contribution: winding number and momentum quantum number label different descriptions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
