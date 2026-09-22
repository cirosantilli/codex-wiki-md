<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Hydrostatic equilibrium and mass conservation are

$$
\frac{dP}{dr}=-\frac{Gm\rho}{r^2},
\qquad
\frac{dm}{dr}=4\pi r^2\rho.
$$

For $P=K\rho^{1+1/n}$, set

$$
\rho=\rho_c\theta^n,\qquad r=a\xi,
\qquad
a^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1}.
$$

Eliminating $m$ gives the [Lane-Emden equation](../../../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}
\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n}.
$$

If $\xi_1$ is its first zero, then

$$
R=a\xi_1,\qquad
M=4\pi a^3\rho_c[-\xi_1^2\theta'(\xi_1)].
$$

Eliminating $\rho_c$ at fixed $K$ gives

$$
\boxed{M^{\,n-1}R^{\,3-n}=C},
$$

so one convenient choice is $\boxed{\alpha=n-1,\ \beta=3-n}$. Equivalently, one may take $\beta=1$ and $\alpha=(n-1)/(3-n)$.

The index $n=0$ describes an incompressible constant-density body, approximating a weakly compressed small rocky planet. The index $n=3/2$ describes a fully convective monatomic ideal gas or nonrelativistic electron degeneracy, as in a low-mass star, brown dwarf, or nonrelativistic white dwarf.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
