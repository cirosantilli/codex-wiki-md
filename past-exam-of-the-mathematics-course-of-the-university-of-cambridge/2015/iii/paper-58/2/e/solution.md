<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a [stellar polytrope](../../../../../../stellar-polytrope.md) of index $n>0$, write $P=K\rho^{1+1/n}$ and combine [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) with [mass conservation](../../../../../../mass-conservation.md) to obtain

$$
\frac1{r^2}\frac d{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G\rho.
$$

Introduce [Lane-Emden variables for a stellar polytrope](../../../../../../lane-emden-variables-for-a-stellar-polytrope.md), $\rho=\rho_c\theta^n$, $P=P_c\theta^{n+1}$ and $r=\alpha\xi$, where

$$
\alpha^2=\frac{(n+1)P_c}{4\pi G\rho_c^2}.
$$

Since $\rho^{-1}dP/dr=(n+1)P_c\theta'/\rho_c\alpha$, the mechanical equation reduces to the [Lane-Emden equation](../../../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^n,\qquad\theta(0)=1,\quad\theta'(0)=0.}
$$

A constant-density interior corresponds to the formal [polytrope of index zero](../../../../../../polytrope-of-index-zero.md), with $\rho=\rho_c\theta^0=\rho_c$ where $\theta>0$. At $n=0$, regularity first gives $\xi^2\theta'=-\xi^3/3$, and a second integration gives

$$
\boxed{\theta(\xi)=1-\frac{\xi^2}{6},\qquad\xi_1=\sqrt6,\qquad R=\alpha\sqrt6.}
$$

Here $P=P_c\theta=P_c(1-r^2/R^2)$ and $\alpha^2=P_c/(4\pi G\rho_c^2)$, reproducing $P_c=2\pi G\rho_c^2R^2/3$. The [mass density](../../../../../../density.md) jumps from its constant interior value to zero at the surface, while [pressure](../../../../../../pressure.md) vanishes continuously. The relation $P=K\rho^{1+1/n}$ is singular at $n=0$; the regular dimensionless [pressure](../../../../../../pressure.md)/[mass density](../../../../../../density.md) formulation defines this incompressible structural limit. It does not mean that the gas's perturbative [stellar adiabatic exponent](../../../../../../stellar-adiabatic-exponent.md) is infinite: the hydrostatic ideal-gas toy model and its adiabatic response are distinct choices.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
