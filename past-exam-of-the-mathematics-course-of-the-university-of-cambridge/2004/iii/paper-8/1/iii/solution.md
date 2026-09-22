<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A field $u(x,t)$ has infinitely many degrees of freedom: its initial state is a [function](../../../../../../function-split.md) rather than a finite list of coordinates. For a [Hamiltonian](../../../../../../hamiltonian.md) evolution, the analogue of the finite-dimensional construction seeks an infinite sequence of independent conserved [functionals](../../../../../../functional.md) $H_j[u]$ whose [Poisson brackets](../../../../../../poisson-bracket.md) vanish. Their [Hamiltonian vector fields](../../../../../../hamiltonian-vector-field.md) then define commuting time evolutions. For example, a [Poisson operator](../../../../../../poisson-operator.md) $J$ produces the field equation $u_t=J\,\delta H/\delta u$, where $\delta H/\delta u$ is the [variational derivative](../../../../../../variational-derivative.md).

A [Lax equation](../../../../../../isospectral-lax-equation.md) packages many conservation laws into one operator identity. If $L_t=[A,L]$, cyclicity of an appropriate trace gives

$$
\frac{d}{dt}\operatorname{Tr}(L^r)
=r\operatorname{Tr}(L^{r-1}[A,L])
=r\operatorname{Tr}([A,L^r])=0.
$$

For a [formal pseudodifferential operator](../../../../../../formal-pseudodifferential-operator.md) the relevant trace is the [Adler trace](../../../../../../adler-trace.md); suitable fractional powers of a monic [differential operator](../../../../../../differential-operator.md) produce further conserved [functionals](../../../../../../functional.md). A [Lenard-Magri recursion](../../../../../../lenard-magri-recursion.md) can prove that such [functionals](../../../../../../functional.md) are [Poisson-commuting functions](../../../../../../poisson-commuting-functions.md), rather than merely [conserved quantities](../../../../../../conserved-quantity.md). A [Lax equation](../../../../../../isospectral-lax-equation.md) by itself does not establish all the independence and completeness properties needed for integrability.

The [Korteweg-De Vries equation](../../../../../../korteweg-de-vries-equation.md) illustrates the mechanism. In one time normalization take $L=\partial^2+u$ and $A=\partial^3+\tfrac32u\partial+\tfrac34u_x$. Direct composition gives

$$
L_t=[A,L]\quad\Longleftrightarrow\quad
u_t=\frac14u_{xxx}+\frac32u u_x.
$$

Its spectral problem, together with the [inverse scattering transform](../../../../../../inverse-scattering-transform.md) for decaying data or suitable spectral coordinates for periodic data, turns nonlinear evolution into simple evolution of spectral data. Solitary waves arise from discrete spectral data, while continuous data describe dispersive radiation.

Thus [infinite-dimensional Hamiltonian integrability](../../../../../../infinite-dimensional-hamiltonian-integrability.md) is more than an infinite list of formulas: one wants sufficiently complete commuting invariants and a reconstruction mechanism that solves the evolution. [Boundary conditions](../../../../../../boundary-condition.md) and the [function](../../../../../../function-split.md) space are essential. A formal hierarchy need not converge, and an infinite family of [conserved quantities](../../../../../../conserved-quantity.md) does not automatically give a compact infinite-dimensional [torus](../../../../../../torus.md) or an unrestricted analogue of the [Arnold-Liouville theorem](../../../../../../liouville-arnold-theorem.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
