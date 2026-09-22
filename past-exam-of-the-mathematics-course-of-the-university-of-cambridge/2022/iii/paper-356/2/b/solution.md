<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0\leq F_0<1$, stationary points satisfy $\cos x=F_0$. There is one minimum $m_k=2\pi-\arccos F_0+2\pi k$ and one maximum $M_k=\arccos F_0+2\pi k$ per period. The potential is a sinusoidal washboard tilted downward to the right by $2\pi F_0$ per period.

Periodization partitions the real line into translated cells, so

$$
\int_{M_0}^{M_1}\widehat p(x,t)dx=\int_{\mathbb R}p(x,t)dx=1.
$$

Translation by $2\pi$ merely reindexes the sum, proving periodic boundary conditions; summing the Fokker--Planck equation proves that $\widehat p$ obeys it.

At stationarity the current $J_0=-D\widehat p_s'-\phi'\widehat p_s$ is constant. Solving this first-order equation and imposing periodicity gives

$$
\boxed{\widehat p_s(x)=\frac{J_0u(x)}{D(1-e^{-2\pi F_0/D})},
\qquad
u(x)=e^{-\phi(x)/D}\int_x^{x+2\pi}e^{\phi(y)/D}dy.}
$$

Here $J_0$ is the stationary probability crossing any point per unit time. Normalization determines it:

$$
\boxed{J_0=\frac{D(1-e^{-2\pi F_0/D})}
{\int_{M_0}^{M_1}u(x)dx}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
