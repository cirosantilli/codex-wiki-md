<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Set $\Delta=T/M$, $q_0=q$, and $q_M=q'$. The [Trotter product formula](../../../../../lie-product-formula.md) separates the kinetic and [potential energy](../../../../../potential-energy.md) evolution to first order in $\Delta$. Inserting $M-1$ resolutions of the identity in the [position operator](../../../../../position-operator.md) basis and using the free short-time kernel gives

$$
K(q',q;T)=\lim_{M\to\infty}(2\pi i\Delta)^{-M/2}
\int\prod_{j=1}^{M-1}dq_j\,
\exp\left\{i\sum_{j=1}^{M}\left[\frac{(q_j-q_{j-1})^2}{2\Delta}-\Delta V(q_{j-1})\right]\right\}.
$$

The exponent converges formally to the [action](../../../../../action.md) along the path. The prefactors and intermediate integrations define the [time-sliced configuration-space path integral](../../../../../time-sliced-configuration-space-path-integral.md) measure, so

$$
\boxed{K(q',q;T)=\int_{q(0)=q}^{q(T)=q'}\mathcal Dq\,e^{iS[q]}.}
$$

A real-time [path integral](../../../../../path-integral.md) is an oscillatory limit with the [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md), rather than an ordinary probability integral. The operator derivation assumes the usual [self-adjointness](../../../../../self-adjoint-operator.md) and product-formula hypotheses for the Hamiltonian.

For a quadratic [potential energy](../../../../../potential-energy.md) write $q=q_c+\eta$, with $\eta(0)=\eta(T)=0$ and $\ddot q_c+V'(q_c)=0$. The first variation vanishes by the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) and the fixed endpoints. Because $V$ is quadratic, the remaining expansion is exact:

$$
S[q_c+\eta]=S[q_c]+\frac12\int_0^T\bigl(\dot\eta^2-V''\eta^2\bigr)dt
=S[q_c]-\frac12\int_0^T\eta A\eta\,dt,
\qquad A=\partial_t^2+V''.
$$

Here [integration by parts](../../../../../integration-by-parts.md) has no boundary contribution. Translation of the integration variables leaves the time-sliced measure unchanged. Thus the [Gaussian path integral](../../../../../gaussian-path-integral.md) over $\eta$ is independent of the endpoint values, and **the entire endpoint dependence lies in $e^{iS[q_c]}$**.

Expanding $\eta$ in [eigenfunctions](../../../../../eigenfunction.md) satisfying [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), each real mode contributes an inverse square root of its quadratic [eigenvalue](../../../../../eigenvalue.md), with the oscillatory phase fixed by continuation. Normalizing against $A_0=\partial_t^2$ gives a precise determinant-ratio form:

$$
\boxed{N(T)=\frac1{\sqrt{2\pi iT}}
\left(\frac{\det_D A}{\det_D A_0}\right)^{-1/2}.}
$$

The [determinant](../../../../../determinant.md) ratio is meaningful after a common regulator; the phase is part of the prescription. It is equivalent to writing $N=C(T)(\det_D A)^{-1/2}$ with an endpoint-independent normalization.

For example, if $V''=\omega^2$, the [Dirichlet oscillator determinant ratio](../../../../../dirichlet-oscillator-determinant-ratio.md) is

$$
\frac{\det_D A}{\det_D A_0}
=\prod_{r=1}^{\infty}\left(1-\frac{\omega^2T^2}{r^2\pi^2}\right)
=\frac{\sin\omega T}{\omega T},
\qquad N=\left(\frac{\omega}{2\pi i\sin\omega T}\right)^{1/2}.
$$

A linear or constant term in $V$ changes the [action](../../../../../action.md) but not this prefactor. The formula holds away from conjugate times, when the boundary problem and [determinant](../../../../../determinant.md) are nonsingular. At $\sin\omega T=0$, it must be continued as a [distribution](../../../../../distribution-mathematical-analysis.md) with its [Maslov index](../../../../../maslov-index.md) phase; the assertion of an ordinary finite prefactor cannot be used literally there. For the unshifted oscillator, at $T=r\pi/\omega$ the kernel is $e^{-ir\pi/2}\delta(q'-(-1)^r q)$.

For the full-line source integral, impose vacuum boundary conditions by adiabatic damping. Take the source initially as a [test function](../../../../../test-function.md), so its pairings with the [Green function](../../../../../green-s-function.md) are defined. After [integration by parts](../../../../../integration-by-parts.md), write

$$
S[q]=\frac12(q,Kq)+(J,q),\qquad K=-\partial_t^2-m^2+i\epsilon.
$$

With the [Fourier transform](../../../../../fourier-transform.md) convention $G(t)=\int d\omega\,e^{i\omega t}\widetilde G(\omega)/(2\pi)$, the inverse is

$$
\widetilde G(\omega)=\frac1{\omega^2-m^2+i\epsilon},\qquad KG=\delta.
$$

Set $q=\eta-GJ$. [Completing the square](../../../../../completing-the-square.md) gives

$$
S[q]=\frac12(\eta,K\eta)-\frac12\int dt\,dt'\,J(t)G(t-t')J(t'),
$$

and consequently

$$
\boxed{Z[J]=Z[0]\exp\left[-\frac i2\int dt\,dt'\,J(t)G(t-t')J(t')\right].}
$$

The [Gaussian functional integral](../../../../../gaussian-functional-integral.md) $Z[0]$ is source independent and contains the regulated [determinant](../../../../../determinant.md). This is most naturally read as a [normalized vacuum generating functional](../../../../../normalized-vacuum-generating-functional.md). For $m>0$, closing the frequency contour gives $G(t)=-i e^{-im|t|}/(2m)$; the time-ordered oscillator two-point function is $iG(t)$. This checks the sign of the source exponent and identifies the required vacuum prescription.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
