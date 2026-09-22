<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

Apply the [curl of the curl identity](../../../../../curl-of-the-curl-identity.md) $\nabla\times(\nabla\times E)=\nabla(\nabla\cdot E)-\nabla^2E$ to [Faraday's law](../../../../../faraday-s-law-of-induction.md), and use the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md). This gives

$$
\boxed{\frac{\partial^2E}{\partial t^2}-\nabla^2E=-\nabla\rho-\frac{\partial J}{\partial t}.}
$$

Applying the same identity to $B$, using $\nabla\cdot B=0$, gives

$$
\boxed{\frac{\partial^2B}{\partial t^2}-\nabla^2B=\nabla\times J.}
$$

For a spherically symmetric charge density, [Gauss's law](../../../../../gauss-s-law.md) on a sphere of radius $r$ gives

$$
E(r)=\frac{\widehat{\mathbf r}}{r^2}\int_0^r\rho(s)s^2\,ds.
$$

For the unit-density ball of radius $a$,

$$
\boxed{
E=\begin{cases}\dfrac r3\widehat{\mathbf r},&r<a,\\[4pt]
\dfrac{a^3}{3r^2}\widehat{\mathbf r},&r\geq a,
\end{cases}
\qquad
\phi=\begin{cases}\dfrac{3a^2-r^2}{6},&r<a,\\[4pt]
\dfrac{a^3}{3r},&r\geq a.
\end{cases}}
$$

The potential is continuous at $r=a$ and tends to zero at infinity.

Let $\mathbf p=(1,0,0)$ and write $\mathbf1_{S_n}$ for the indicator of $S_n$. The layered density decomposes as

$$
\rho=\mathbf1_{S_0}+\sum_{n\geq1}2^{n-1}\mathbf1_{S_n}.
$$

The point $\mathbf p$ lies on every sphere $S_n$, whose radius is $R_n=4^{-n}$ and whose outward radial direction there is $\widehat{\mathbf x}$. A uniform ball of density $c$ contributes $cR_n/3$ to the field and $cR_n^2/3$ to the potential at its surface. Therefore

$$
E(\mathbf p)=\frac13\left(1+\sum_{n\geq1}2^{n-1}4^{-n}\right)\widehat{\mathbf x}
=\boxed{\frac12\widehat{\mathbf x}},
$$

and

$$
\phi(\mathbf p)=\frac13\left(1+\sum_{n\geq1}2^{n-1}16^{-n}\right)
=\boxed{\frac5{14}}.
$$

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
