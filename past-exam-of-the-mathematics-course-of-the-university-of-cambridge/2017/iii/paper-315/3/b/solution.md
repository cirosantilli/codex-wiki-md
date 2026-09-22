<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume a Newtonian, spherically symmetric, nonrotating body in [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md), supported by a [polytropic equation of state](../../../../../../polytropic-equation-of-state.md) $P=K\rho^{1+1/n}$ with constant $K>0$ and $n>0$. The [enclosed mass](../../../../../../enclosed-mass.md) and [hydrostatic pressure support equation](../../../../../../hydrostatic-pressure-support-equation.md) are

$$
\frac{dm}{dr}=4\pi r^2\rho,\qquad
\frac{dP}{dr}=-\frac{Gm\rho}{r^2}.
$$

Eliminate $m$ by first writing $r^2\rho^{-1}dP/dr=-Gm$ and then differentiating:

$$
\frac1{r^2}\frac{d}{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)
=-4\pi G\rho.
$$

Let $\rho_c$ be central [mass density](../../../../../../density.md), and introduce the [Lane-Emden variables for a stellar polytrope](../../../../../../lane-emden-variables-for-a-stellar-polytrope.md)

$$
\rho=\rho_c\theta^n,\qquad
P=K\rho_c^{1+1/n}\theta^{n+1},\qquad
r=a\xi,
$$

where

$$
a^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1}.
$$

Then $(1/\rho)dP/dr=(n+1)K\rho_c^{1/n}d\theta/dr$. Substitution cancels the dimensional factors and yields the [Lane-Emden equation](../../../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac{d}{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)
=-\theta^n,\qquad \theta(0)=1,\quad\theta'(0)=0.}
$$

The central conditions enforce the chosen central [mass density](../../../../../../density.md) and regular [spherical symmetry](../../../../../../spherical-symmetry.md). The local regular expansion is $\theta=1-\xi^2/6+n\xi^4/120+\cdots$. If a finite first zero $\xi_1$ exists and surface [pressure](../../../../../../pressure.md) is negligible, the physical [radius](../../../../../../radius.md) is $R=a\xi_1$, and the [Lane-Emden mass formula](../../../../../../lane-emden-mass-formula.md) is $M=4\pi a^3\rho_c[-\xi_1^2\theta'(\xi_1)]$. For $0<n<5$ the standard isolated solution has a finite surface; $n=5$ has infinite extent, so a finite surface must not be assumed for all indices. Irradiation, composition stratification and non-polytropic equations of state require more general structure equations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
