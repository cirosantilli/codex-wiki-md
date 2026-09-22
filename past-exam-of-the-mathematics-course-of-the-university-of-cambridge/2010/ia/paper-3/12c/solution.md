<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

For a [spherically symmetric potential](../../../../../spherically-symmetric-potential.md), the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) becomes

$$
\frac1{r^2}\frac{d}{dr}\left(r^2\phi'(r)\right)=4\pi G\rho(r).
$$

Integrate from the center, excluding any additional point mass there. The boundary condition is $r^2\phi'(r)\to0$ as $r\to0$, so

$$
r^2\phi'(r)=4\pi G\int_0^r\rho(s)s^2\,ds=GM(r),\qquad \mathbf g(r)=-\frac{GM(r)}{r^2}\widehat{\mathbf r}.
$$

This derives the enclosed-mass form of the [spherical shell theorem](../../../../../spherical-shell-theorem.md) from the differential equation. Outside the mass, integrating $\phi'=GM/r^2$ gives $\phi=-GM/r+C$; the conventional zero at infinity sets $C=0$.

For the dyadic shells, multiply their constant [mass density](../../../../../density.md) by their spherical volumes. The $n$th shell contributes

$$
\begin{aligned}
M_n&=\frac{4\pi}{3}\rho_0\,2^{n-1}\left(2^{3-3n}-2^{-3n}\right)\\
&=\frac{14\pi\rho_0}{3}\,4^{-n}.
\end{aligned}
$$

Summing the [geometric series](../../../../../geometric-series.md) yields

$$
\boxed{M=\sum_{n=1}^\infty M_n=\frac{14\pi\rho_0}{9}.}
$$

At radius $r=2^{-N}$, the enclosed shells are exactly those with $n\geq N+1$; a boundary itself contributes no mass. Thus

$$
M(2^{-N})=\frac{14\pi\rho_0}{3}\sum_{n=N+1}^\infty4^{-n}=\frac{14\pi\rho_0}{9}\,4^{-N}.
$$

Dividing by $r^2=4^{-N}$ gives

$$
\boxed{\mathbf g(2^{-N})=-\frac{14\pi G\rho_0}{9}\widehat{\mathbf r}\qquad(N\geq1).}
$$

These [dyadic spherical shells with inverse-radius density scaling](../../../../../dyadic-spherical-shells-with-inverse-radius-density-scaling.md) have the same field magnitude at each shell boundary, although the field varies inside an individual shell. Finally, outside the planet,

$$
\boxed{\phi(r)=-\frac{14\pi G\rho_0}{9r}\qquad(r>1),}
$$

with zero potential at infinity; without that convention an arbitrary additive constant remains.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
