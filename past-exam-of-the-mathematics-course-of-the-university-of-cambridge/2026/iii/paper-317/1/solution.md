<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [stellar polytrope](../../../../../stellar-polytrope.md) of index $n$ obeys

$$
P=K\rho^{1+1/n},
\qquad
\rho=\rho_c\theta^n,
\qquad
r=\alpha\xi.
$$

Combining [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md), $dP/dr=-Gm\rho/r^2$, with mass conservation, $dm/dr=4\pi r^2\rho$, gives the [Lane-Emden equation](../../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}
\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n},
\qquad
\boxed{\alpha^2=\frac{(n+1)K}{4\pi G}
\rho_c^{1/n-1}}.
$$

Regularity and normalization at the stellar centre require

$$
\boxed{\theta(0)=1,\qquad\theta'(0)=0}.
$$

Integrating the Lane-Emden equation from the centre then gives the enclosed mass

$$
\boxed{m(r)=-4\pi\rho_c\alpha^3\xi^2\theta'(\xi)}.
$$

For $n=5$, direct substitution into the equation finds

$$
\boxed{\theta=(1+\xi^2/3)^{-1/2}},
$$

so $\beta=1/3$ and $\gamma=-1/2$. This profile has no finite first zero and hence has infinite radius, but its total mass converges:

$$
\boxed{M=4\pi\sqrt3\,\rho_c\alpha^3}.
$$

Its mean density over the full, infinite configuration is consequently zero.

For a perfect gas, $T\propto P/\rho\propto\rho^{1/5}$, so $T/T_c=\theta$. The luminosity from [CNO cycle](../../../../../cno-cycle.md) burning with $\epsilon=\epsilon_0\rho T^{11}$ is therefore

$$
L=4\pi\epsilon_0\alpha^3\rho_c^2T_c^{11}
\int_0^\infty\xi^2\theta^{21}\,d\xi
=A\epsilon_0\alpha^3\rho_c^2T_c^{11},
$$

where

$$
A=4\pi\int_0^\infty\xi^2(1+\xi^2/3)^{-21/2}d\xi
=6\pi\sqrt3\,B(3/2,9)\simeq1.03.
$$

Thus $A$ is of order unity. The model is physically poor because the $n=5$ polytrope has infinite radius and zero mean density, while strongly temperature-sensitive CNO burning changes the thermal gradient and commonly creates convection. Real cores also have evolving composition, non-polytropic opacity and energy transport, and boundaries supplied by the surrounding star.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
