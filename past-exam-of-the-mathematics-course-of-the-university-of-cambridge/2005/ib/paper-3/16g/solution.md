<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

For an axisymmetric potential, insert $\Psi(r,\phi)=R(r)\Phi(\phi)$ into the time-independent [Schrödinger equation](../../../../../schrodinger-equation.md) and divide by $R\Phi$. The polar [Laplacian](../../../../../laplacian.md) separates the angular equation $\Phi''+m^2\Phi=0$ from

$$
R''+\frac1rR'+\left[\frac{2\mu(E-V(r))}{\hbar^2}-\frac{m^2}{r^2}\right]R=0.
$$

Single-valuedness under $\phi\mapsto\phi+2\pi$ gives $m\in\mathbb Z$, with an angular eigenbasis $\boxed{\Phi=e^{im\phi}}$. Linear combinations of the degenerate $m,-m$ modes are also possible.

Inside the [circular infinite quantum well](../../../../../circular-infinite-quantum-well.md), put $\rho=r\sqrt{2\mu E/\hbar^2}$. The equation becomes

$$
\boxed{R_{\rho\rho}+\rho^{-1}R_\rho+(1-m^2/\rho^2)R=0}.
$$

The physical solution must be regular at the origin, behaving as $r^{|m|}$ for $m\ne0$, or with finite value and zero radial derivative for $m=0$. At the infinite wall impose $R(r=a)=0$. The printed question's boundary phrase uses capital $R=a$; it means the radial position $r=a$, not a value imposed on the radial wavefunction. The singular [Bessel function of the second kind](../../../../../bessel-function-of-the-second-kind.md) is excluded; mere square-integrability of its logarithmic $m=0$ singularity would not put it in the ordinary finite-energy Hamiltonian domain.

For $m=0$, multiply the equation by $\rho^2$ and insert $R=\sum_{k\geq0}A_k\rho^k$. The coefficient of $\rho$ gives $A_1=0$, and subsequent coefficients give

$$
\boxed{A_{k+2}=-\frac{A_k}{(k+2)^2}}.
$$

All odd coefficients vanish, $A_2=-A_0/4$, and $A_4=A_0/64$. The regular solution is a multiple of the [Bessel function of the first kind](../../../../../bessel-function-of-the-first-kind.md) $J_0$. Its requested fourth-order estimate is

$$
R(\rho)\approx A_0(1-\rho^2/4+\rho^4/64)=A_0(1-\rho^2/8)^2.
$$

Therefore the first positive zero of this truncation is $\boxed{\rho\approx\sqrt8}$, giving

$$
\boxed{E_0\approx\frac{\hbar^2(\sqrt8)^2}{2\mu a^2}=\frac{4\hbar^2}{\mu a^2}}.
$$

The ground state is in the $m=0$ sector because nonzero angular modes add nonnegative centrifugal kinetic energy to the radial energy form. This [quartic truncation of the Bessel function J0](../../../../../quartic-truncation-of-the-bessel-function-j0.md) is only a rough local-series estimate, not an exact eigenvalue or a certified variational bound; its double zero warns that the truncation does not reproduce the simple zero of the full function.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
