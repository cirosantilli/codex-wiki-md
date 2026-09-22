<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in units $\hbar=1$ and with the particle [mass](../../../../../mass.md) absorbed into the stated kinetic term. Divide the interval into $N$ pieces of length $\Delta=T/N$. For a suitable self-adjoint [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), the [Trotter product formula](../../../../../lie-product-formula.md) gives the regulated limit

$$
e^{-i\hat HT}=\lim_{N\to\infty}\left(e^{-i\Delta\hat p^2/2}e^{-i\Delta V(\hat q)}\right)^N.
$$

Insert $1=\int dq_j\,|q_j\rangle\langle q_j|$ between neighboring factors. Because $V(\hat q)$ is diagonal in the [position operator](../../../../../position-operator.md) basis, the given [free-particle propagator](../../../../../free-particle-propagator.md) yields

$$
\begin{aligned}
K(q',q;T)
&=\lim_{N\to\infty}(2\pi i\Delta)^{-N/2}\int\prod_{j=1}^{N-1}dq_j\,
\exp\left[i\sum_{j=0}^{N-1}\left\{\frac{(q_{j+1}-q_j)^2}{2\Delta}-\Delta V(q_j)\right\}\right],\\
q_0&=q,\qquad q_N=q'.
\end{aligned}
$$

The exponent is the time-sliced [action](../../../../../action.md). Its continuum notation is

$$
\boxed{K(q',q;T)=\int_{q(0)=q}^{q(T)=q'}\mathcal Dq\,e^{iS[q]},\qquad
S[q]=\int_0^T\left(\frac12\dot q^2-V(q)\right)dt.}
$$

The measure is defined by the displayed finite-dimensional limits and their normalization, not by a translation-invariant flat measure on an infinite-dimensional space. The oscillatory limit needs a damping/analytic-continuation prescription. This is the [time-sliced configuration-space path integral](../../../../../time-sliced-configuration-space-path-integral.md) derived from the operator kernel.

For a quadratic [potential energy](../../../../../potential-energy.md), write $q=q_c+\eta$, where the [classical path](../../../../../classical-path.md) satisfies $\ddot q_c+V'(q_c)=0$ and the endpoint conditions, and $\eta(0)=\eta(T)=0$. Expansion is exact:

$$
S[q_c+\eta]=S[q_c]+\int_0^T(\dot q_c\dot\eta-V'(q_c)\eta)dt
+\frac12\int_0^T(\dot\eta^2-V''\eta^2)dt.
$$

[Integration by parts](../../../../../integration-by-parts.md) makes the linear term equal to $-[\int_0^T(\ddot q_c+V'(q_c))\eta\,dt]$, since the endpoint term vanishes. It is zero by the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). Also $V''$ is constant, independent of the endpoints. Thus [classical-path factorization of a quadratic path integral](../../../../../classical-path-factorization-of-a-quadratic-path-integral.md) is exact:

$$
\boxed{K(q',q;T)=N(T)e^{iS[q_c]},\qquad
N(T)=\int_{\eta(0)=\eta(T)=0}\mathcal D\eta\,
\exp\left[-\frac i2\int_0^T\eta\left(\frac{d^2}{dt^2}+V''\right)\eta\,dt\right].}
$$

Only the classical [action](../../../../../action.md) carries the endpoint dependence.

Let $D=\partial_t^2+V''$ on homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). Expand $\eta$ in its normalized eigenfunctions, with [eigenvalues](../../../../../eigenvalue.md) $\lambda_n$. The fluctuation integral becomes a product of regulated integrals $\int da_n\exp(-i\lambda_na_n^2/2)$. Each is proportional to $\lambda_n^{-1/2}$, with a prescribed complex phase. Relative to $D_0=\partial_t^2$, the normalization is therefore

$$
\boxed{N(T)=\frac1{\sqrt{2\pi iT}}\left(\frac{\det_D D}{\det_D D_0}\right)^{-1/2}.}
$$

The subscript denotes the Dirichlet operator domain, and the square-root branch is continued from the free kernel with its convergence prescription. Equivalently one can use [determinants](../../../../../determinant.md) of $-D$ and $-D_0$. For $V''=\omega^2$, the [Dirichlet oscillator determinant ratio](../../../../../dirichlet-oscillator-determinant-ratio.md) is

$$
\prod_{n=1}^{\infty}\left(1-\frac{\omega^2T^2}{\pi^2n^2}\right)
=\frac{\sin\omega T}{\omega T},\qquad
N(T)=\left(\frac{\omega}{2\pi i\sin\omega T}\right)^{1/2}.
$$

This also checks the free limit. At conjugate times, the fluctuation operator has a zero [eigenvalue](../../../../../eigenvalue.md) and the ordinary finite-prefactor expression fails; the kernel is obtained by distributional continuation. Away from these times the classical boundary problem is unique and the stated factorization applies directly.

For the infinite-time oscillator with an [external source](../../../../../source-quantum-field-theory.md), use vacuum boundary conditions and the [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md). For a smooth [source](../../../../../source-quantum-field-theory.md) of compact support, define

$$
A_\epsilon=-\partial_t^2-m^2+i\epsilon,\qquad
G_\epsilon=A_\epsilon^{-1},\qquad\epsilon>0.
$$

The imaginary term damps the real-field integral. Integration by parts gives $S_\epsilon[q]=\tfrac12qA_\epsilon q+Jq$, with the pairings understood as time integrals. [Completing the square](../../../../../completing-the-square.md) gives

$$
\frac12qA_\epsilon q+Jq
=\frac12(q+G_\epsilon J)A_\epsilon(q+G_\epsilon J)-\frac12JG_\epsilon J.
$$

Translate the integration variable. The source-independent [Gaussian functional integral](../../../../../gaussian-functional-integral.md) is $N$, so

$$
\boxed{\int\mathcal Dq\,e^{iS[q]}=N\exp\left[-\frac i2\int dt\,dt'\,J(t)G(t-t')J(t')\right].}
$$

On [Fourier modes](../../../../../fourier-mode.md) $e^{i\omega t}$, $A_\epsilon$ has [eigenvalue](../../../../../eigenvalue.md) $\omega^2-m^2+i\epsilon$, hence

$$
\boxed{G(t)=\lim_{\epsilon\downarrow0}\frac1{2\pi}\int_{\mathbb R}\frac{e^{i\omega t}}{\omega^2-m^2+i\epsilon}\,d\omega.}
$$

For $m>0$, closing the contour above for $t>0$ and below for $t<0$ gives $G(t)=-ie^{-im|t|}/(2m)$. The physical time-ordered oscillator [quantum field theory propagator](../../../../../propagator.md) is $iG$, not $G$ itself. The shifted stationary path is $q_c=-GJ$ and obeys $\ddot q_c+m^2q_c=J$ with the same vacuum prescription. A retarded inverse would define a different boundary problem. Dividing by the zero-source integral removes $N$ and gives the [vacuum source functional of a quantum oscillator](../../../../../vacuum-source-functional-of-a-quantum-oscillator.md). At zero [mass](../../../../../mass.md) an additional infrared prescription is needed for the inverse on constant modes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
