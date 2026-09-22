<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For constant $B_z$, [cylindrical magnetostatic pressure balance](../../../../../../cylindrical-magnetostatic-pressure-balance.md) gives

$$
\frac{dI^2}{dR}=-2\pi c^2R^2\frac{dp}{dR}
=\frac{4\pi c^2kp_0R^3}{a^2}\left(1+\frac{R^2}{a^2}\right)^{-k-1}.
$$

Regularity gives $I(0)=0$. With $x=R^2/a^2$, integration yields the [power-law pressure-supported axial current](../../../../../../power-law-pressure-supported-axial-current.md)

$$
\boxed{I^2(R)=2\pi c^2p_0a^2
\begin{cases}
\displaystyle\frac{1-(1+kx)(1+x)^{-k}}{k-1},&k\ne1,\\
\log(1+x)+(1+x)^{-1}-1,&k=1.
\end{cases}}
$$

The sign of $I$ may be chosen either way and fixes the sense of the [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md). For $p_0>0$ and nontrivial decreasing [pressure](../../../../../../pressure.md) ($k>0$), the integral converges at infinity precisely when

$$
\boxed{k>1,\qquad I^2(\infty)=\frac{2\pi c^2p_0a^2}{k-1}.}
$$

At $k=1$ it diverges logarithmically; for $0<k<1$ it diverges as $R^{2(1-k)}$. The degenerate case $k=0$ has constant [pressure](../../../../../../pressure.md) and zero [electric current](../../../../../../electric-current.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
