<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) in this question is already in thermal units, as indicated by $e^{-H}$ without an additional $\beta_T$. Define $W[h]=\log Z[h]$ and $F[h]=-W[h]$. The mean field and its linear response are

$$
m_h(x)=\frac{\delta W}{\delta h(x)}=-\frac{\delta F}{\delta h(x)},\qquad
G(x,y)=\frac{\delta m_h(x)}{\delta h(y)}
=\langle\phi(x)\phi(y)\rangle-\langle\phi(x)\rangle\langle\phi(y)\rangle.
$$

These are [functional derivatives](../../../../../../functional-derivative.md) of the [connected generating functional](../../../../../../connected-generating-functional.md); the subtraction defines the [connected correlation function](../../../../../../connected-correlation-function.md). In the [Landau approximation](../../../../../../landau-approximation.md), neglect loop corrections and evaluate the field integral at a stable saddle $m_h$. It satisfies the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md)

$$
\boxed{-\nabla^2m_h(x)+r_0m_h(x)+\frac{u_0}{6}m_h(x)^3=h(x).}
$$

This follows by varying the [gradient](../../../../../../gradient.md) term and integrating by parts, with periodic, decaying, or otherwise appropriate boundary conditions.

The two requested [free energy](../../../../../../thermodynamic-free-energy.md) functionals, following the source and Legendre conventions of the question, are

$$
\boxed{F_{\mathrm L}[h]=H[m_h,h],\qquad
\Gamma_{\mathrm L}[m]=F_{\mathrm L}[h]+\int d^Dx\,h(x)m(x)
=\int d^Dx\left[\frac12(\nabla m)^2+\frac12r_0m^2+\frac{u_0}{4!}m^4\right].}
$$

In the [scalar-field source Legendre transform](../../../../../../scalar-field-source-legendre-transform.md) on the chosen stable branch, $h$ is chosen to produce $m$, and $\delta\Gamma_{\mathrm L}/\delta m=h$. Thus the imposed-source [Helmholtz free energy](../../../../../../helmholtz-free-energy.md) and the fixed-order-parameter [Gibbs free energy](../../../../../../gibbs-free-energy.md) have the appropriate opposite source derivatives. These names are used in the question's magnetic-ensemble convention; the defining sign relation is what fixes the calculation. At leading [Landau approximation](../../../../../../landau-approximation.md) there is no fluctuation-determinant term in $F_{\mathrm L}$.

Differentiate the saddle equation with respect to $h(y)$. The response obeys

$$
\boxed{\left[-\nabla_x^2+r_0+\frac{u_0}{2}m_h(x)^2\right]G(x,y)
=\delta^{(D)}(x-y).}
$$

Therefore

$$
\boxed{K(x)=-\nabla_x^2+r_0+\frac{u_0}{2}m_h(x)^2.}
$$

Equivalently, the [inverse Hessian relation for a connected two-point function](../../../../../../inverse-hessian-relation-for-a-connected-two-point-function.md) states that $G$ is the inverse kernel of $\delta^2\Gamma_{\mathrm L}/\delta m(x)\delta m(y)$. The factor $u_0/2$ follows from twice differentiating the quartic term $u_0m^4/4!$; it is not $u_0/6$. This tree-level connected response is obtained by varying the saddle. It does not require replacing the exact connected correlator by a product of the saddle values, which would incorrectly give zero.

For the requested single-momentum formula, assume a homogeneous source and a translationally invariant equilibrium phase, so $m_h(x)=m_0$ and $G(x,y)=G(x-y)$. Set

$$
M^2=r_0+\frac{u_0}{2}m_0^2>0.
$$

The [Fourier transform](../../../../../../fourier-transform.md) with the printed positive sign sends $-\nabla^2$ to $q^2$, while the [Dirac delta function](../../../../../../dirac-delta-function.md) transforms to one. Hence the [Ornstein--Zernike correlation function](../../../../../../ornstein-zernike-correlation-function.md) has

$$
\boxed{\widetilde G(q)=\frac{1}{q^2+M^2}
=\frac{1}{q^2+\xi^{-2}},\qquad
\xi=\left(r_0+\frac{u_0}{2}m_0^2\right)^{-1/2}.}
$$

The inverse convention is $G(x)=\int d^Dq\,(2\pi)^{-D}e^{-iq\cdot x}\widetilde G(q)$. For general inhomogeneous $h(x)$, $K$ has nonconstant coefficients and $G$ depends separately on its two positions; the displayed momentum-diagonal formula then does not follow. The preceding differential equation still holds in that case.

At zero source and for $u_0>0$, the homogeneous saddle is $m_0=0$ for $r_0>0$, and $m_0^2=-6r_0/u_0$ on either selected stable ordered branch for $r_0<0$. Thus the [Landau scalar correlation length](../../../../../../landau-scalar-correlation-length.md) is

$$
\boxed{\xi=\begin{cases}r_0^{-1/2},&r_0>0,\\(-2r_0)^{-1/2},&r_0<0.\end{cases}}
$$

In the ordered phase the negative bare quadratic coefficient is compensated by the positive curvature at the nonzero saddle. Retaining $m_0=0$ below the transition would instead give an unstable kernel and is not a physical [correlation length](../../../../../../correlation-length.md). With the usual analytic thermal tuning $r_0=a_0(T-T_c)$, $a_0>0$, both branches diverge as $|T-T_c|^{-1/2}$, so the [correlation-length critical exponent](../../../../../../correlation-length-critical-exponent.md) is

$$
\boxed{\nu_{\mathrm{Landau}}=\frac12.}
$$

The high-temperature amplitude is $\sqrt2$ times the low-temperature amplitude for the same $a_0$. This statement is within [Landau theory](../../../../../../landau-theory.md); fluctuations can change critical behavior outside the mean-field regime.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
