<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [natural units](../../../../../natural-units.md) and the [Minkowski metric](../../../../../minkowski-metric.md) $\eta=\operatorname{diag}(1,-1,-1,-1)$. A [real scalar field](../../../../../real-scalar-field.md) assigns a real variable $\phi(t,\mathbf x)$ to each spatial point. Its [Lagrangian density](../../../../../lagrangian-density.md) can be taken to be

$$
\mathcal L=\frac12\partial_\mu\phi\,\partial^\mu\phi-V(\phi)=\frac12\dot\phi^2-\frac12|\nabla\phi|^2-V(\phi),\qquad S[\phi]=\int d^4x\,\mathcal L.
$$

The [principle of stationary action](../../../../../principle-of-stationary-action.md) gives the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) $\Box\phi+V'(\phi)=0$. With $V(\phi)=m^2\phi^2/2$, this is the [Klein-Gordon equation](../../../../../klein-gordon-equation.md). An additional nonlinear part of $V$ describes interactions.

The [canonical momentum](../../../../../canonical-momentum.md) is $\pi=\partial\mathcal L/\partial\dot\phi=\dot\phi$. The [Legendre transform in mechanics](../../../../../legendre-transform-in-mechanics.md) gives the [canonical Hamiltonian density of a real scalar field](../../../../../canonical-hamiltonian-density-of-a-real-scalar-field.md)

$$
\mathcal H=\pi\dot\phi-\mathcal L=\frac12\pi^2+\frac12|\nabla\phi|^2+V(\phi),\qquad H=\int d^3x\,\mathcal H.
$$

The [Hamiltonian](../../../../../hamiltonian.md) equations $\dot\phi=\pi$ and $\dot\pi=\nabla^2\phi-V'(\phi)$ recover the same field equation. In [canonical quantization](../../../../../canonical-quantization.md), the fields become operators satisfying the equal-time [canonical commutation relations](../../../../../canonical-commutation-relation.md)

$$
[\widehat\phi(t,\mathbf x),\widehat\pi(t,\mathbf y)]=i\delta^3(\mathbf x-\mathbf y),\qquad[\widehat\phi,\widehat\phi]=[\widehat\pi,\widehat\pi]=0.
$$

A spatial lattice makes the analogy with many coupled quantum-mechanical coordinates precise. Each lattice field value is a coordinate, with its own [conjugate momentum](../../../../../canonical-momentum.md). The [path integral](../../../../../path-integral.md) is another representation of the same quantum evolution.

To see its origin, first consider one coordinate with $H=p^2/(2M)+V(q)$. Split a time interval into $N$ steps of length $\varepsilon$ and insert position and momentum resolutions of the identity. The short-time kernel is

$$
\langle q_{j+1}|e^{-i\varepsilon\widehat H}|q_j\rangle=\int\frac{dp_j}{2\pi}\exp\left\{ip_j(q_{j+1}-q_j)-i\varepsilon\left[\frac{p_j^2}{2M}+V(q_j)\right]\right\}+O(\varepsilon^2).
$$

Multiplying the kernels and integrating over intermediate positions gives the [phase-space path integral](../../../../../phase-space-path-integral.md)

$$
K(q_f,t_f;q_i,t_i)=\int\mathcal Dq\,\mathcal Dp\,\exp\left[i\int_{t_i}^{t_f}(p\dot q-H(p,q))\,dt\right].
$$

The endpoints of $q$ are fixed. The momentum integrals are [Gaussian integrals](../../../../../gaussian-integral.md); completing the square produces the [configuration-space path integral](../../../../../configuration-space-path-integral.md)

$$
\boxed{K(q_f,t_f;q_i,t_i)=\int_{q_i}^{q_f}\mathcal Dq\,e^{iS[q]},\qquad S[q]=\int_{t_i}^{t_f}\left(\frac M2\dot q^2-V(q)\right)dt.}
$$

At finite slicing its normalization contains $(M/(2\pi i\varepsilon))^{N/2}\prod_{j=1}^{N-1}dq_j$. This fixes the composition law and the initial delta-function kernel. One sums over all paths, not merely solutions of the classical equation. Restoring $\hbar$ replaces the weight by $e^{iS/\hbar}$; stationary phase explains the emergence of classical trajectories.

For the field, use [scalar field configuration eigenstates](../../../../../scalar-field-configuration-eigenstate.md) $|\varphi\rangle$, satisfying $\widehat\phi(\mathbf x)|\varphi\rangle=\varphi(\mathbf x)|\varphi\rangle$. Insert their completeness relations on every time slice. This gives

$$
\langle\varphi_f|e^{-i\widehat H(t_f-t_i)}|\varphi_i\rangle=\int\mathcal D\phi\,\mathcal D\pi\,\exp\left[i\int d^4x\,(\pi\dot\phi-\mathcal H)\right].
$$

The endpoint field configurations are fixed. Integrating the Gaussian momentum variables leaves the [scalar field path integral](../../../../../scalar-field-path-integral.md) $\mathcal N\int\mathcal D\phi\,e^{iS[\phi]}$. The [functional measure](../../../../../functional-measure.md) means a regulated product over the field variables. A spacetime lattice or another [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) makes this product finite before the continuum limit; interacting continuum calculations may require [renormalization](../../../../../renormalization.md). The oscillatory Minkowski weight is an amplitude, not a positive [probability density](../../../../../probability-density.md).

For [vacuum expectation values](../../../../../vacuum-expectation-value.md), the boundaries must select the vacuum rather than arbitrary field configurations. Long imaginary-time evolution suppresses excited states: $e^{-TH}|n\rangle=e^{-TE_n}|n\rangle$, so after normalization only the lowest-energy component remains as $T\to\infty$. This is [vacuum projection by imaginary time](../../../../../vacuum-projection-by-imaginary-time.md). The corresponding [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) in the real-time integral specifies the vacuum boundary conditions and the poles of the propagator. With $t=-i\tau$, the [Euclidean path integral](../../../../../euclidean-path-integral.md) has the weight $e^{-S_E}$, where

$$
S_E=\int d\tau\,d^3x\left[\frac12(\partial_\tau\phi)^2+\frac12|\nabla\phi|^2+V(\phi)\right].
$$

It is often a useful regulated starting point; analytic continuation returns the vacuum time-ordered quantities.

Introduce a classical source $J(x)$ and define the [normalized vacuum generating functional](../../../../../normalized-vacuum-generating-functional.md)

$$
Z[J]=\frac{\int\mathcal D\phi\,\exp i\left(S[\phi]+\int d^4x\,J(x)\phi(x)\right)}{\int\mathcal D\phi\,e^{iS[\phi]}},\qquad Z[0]=1,
$$

with the same vacuum prescription in numerator and denominator. A [functional derivative](../../../../../functional-derivative.md) brings down $i\phi(x)$. The order of the time slices makes the operator insertion time-ordered. Thus [source differentiation inserts time-ordered field operators](../../../../../source-differentiation-inserts-time-ordered-field-operators.md):

$$
\boxed{\langle\Omega|T\{\widehat\phi(x_1)\cdots\widehat\phi(x_r)\}|\Omega\rangle=\left.\frac1{i^r}\frac{\delta^rZ[J]}{\delta J(x_1)\cdots\delta J(x_r)}\right|_{J=0}.}
$$

The denominator removes vacuum diagrams and gives normalized expectation values. It is essential that these are [time-ordered products](../../../../../time-ordered-product.md); differentiating this vacuum functional does not directly give every possible operator ordering.

The free theory illustrates the method. Its quadratic kernel is $K=-\Box-m^2$ with the vacuum pole prescription, and completing the square gives the [Gaussian evaluation of a free scalar generating functional](../../../../../gaussian-evaluation-of-a-free-scalar-generating-functional.md)

$$
Z_0[J]=\exp\left[-\frac12\int d^4x\,d^4y\,J(x)\Delta_F(x-y)J(y)\right],\qquad \Delta_F(x-y)=\int\frac{d^4p}{(2\pi)^4}\frac{i\,e^{-ip\cdot(x-y)}}{p^2-m^2+i0}.
$$

Two source derivatives give $\Delta_F=\langle\Omega|T\{\widehat\phi(x)\widehat\phi(y)\}|\Omega\rangle$. Higher derivatives give all pairings, the content of [Wick theorem](../../../../../wick-s-theorem.md). For an interaction $S_{\rm int}$, one may use [path-integral perturbation by source derivatives](../../../../../path-integral-perturbation-by-source-derivatives.md):

$$
Z[J]=\frac{\exp\left(iS_{\rm int}\left[\frac1i\frac\delta{\delta J}\right]\right)Z_0[J]}{\left.\exp\left(iS_{\rm int}\left[\frac1i\frac\delta{\delta J}\right]\right)Z_0[J]\right|_{J=0}}.
$$

Expanding this expression generates [Feynman diagrams](../../../../../feynman-diagram.md) and their [Wick contractions](../../../../../wick-contraction.md). The [connected generating functional](../../../../../connected-generating-functional.md) $W[J]=-i\log Z[J]$ retains connected contributions; in particular $\delta W/\delta J=\langle\phi\rangle_J$. These functionals turn the computation of field-operator expectations into source differentiation of an ordinary regulated integral.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
