<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the prepoint prescription for the separable [Hamiltonian](../../../../../../hamiltonian.md). Its regulated exponent is

$$
\sum_{i=1}^N\left[ip_i(q_{i+1}-q_i)-\Delta t_i\left(\frac{p_i^2}{2m}+V(q_i)\right)\right].
$$

Each momentum integration is an ordinary [Gaussian integral](../../../../../../gaussian-integral.md):

$$
\int_{-\infty}^\infty dp_i\,e^{-\Delta t_i p_i^2/(2m)+ip_i(q_{i+1}-q_i)}
=\sqrt{\frac{2\pi m}{\Delta t_i}}\exp\left[-\frac{m(q_{i+1}-q_i)^2}{2\Delta t_i}\right].
$$

Therefore the measure written in the question gives exactly

$$
\boxed{\mathcal Dq_{\mathrm{raw},N}=\prod_{i=1}^N\sqrt{\frac{2\pi m}{\Delta t_i}}\,dq_i,\qquad
S_{E,N}=\sum_{i=1}^N\left[\frac{m(q_{i+1}-q_i)^2}{2\Delta t_i}+\Delta t_i V(q_i)\right].}
$$

The resulting configuration integral is $\int\mathcal Dq_{\mathrm{raw},N}e^{-S_{E,N}}$. This is [Gaussian momentum integration in a phase-space path integral](../../../../../../gaussian-momentum-integration-in-a-phase-space-path-integral.md). Formally its exponent tends to the usual Euclidean kinetic-plus-potential action, but the slice-dependent factors in the measure must be retained.

For a normalized [quantum-mechanical propagator](../../../../../../quantum-mechanical-propagator.md), Fourier completeness uses $dp_i/(2\pi)$ rather than $dp_i$. With that normalization the configuration measure is

$$
\boxed{\mathcal Dq_N=\prod_{i=1}^N\sqrt{\frac{m}{2\pi\Delta t_i}}\,dq_i.}
$$

This differs from the raw measure by $(2\pi)^{-N}$. It makes the free single-step kernel integrate to one and tend to a delta distribution as the interval tends to zero. In these formulas $q_{N+1}$ is fixed and $q_1,\ldots,q_N$ are integrated for propagation from an initial [wavefunction](../../../../../../wave-function.md). If both endpoints are fixed, omit $dq_1$ while retaining its slice normalization factor. The continuum expression means the limit of these measures and exponents, not a flat product of $dq(t)$ with no time-step weights.

We now address the unheaded real-time continuation. Set $m=\hbar=1$. The [normalized short-time Schrödinger kernel](../../../../../../normalized-short-time-schrodinger-kernel.md) gives the final-slice recurrence

$$
\psi(q,t+\Delta t)=\frac1{\sqrt{2\pi i\Delta t}}\int_{-\infty}^{\infty}dq'\,
\exp\left[\frac{i(q-q')^2}{2\Delta t}-i\Delta t V(q')\right]\psi(q',t).
$$

The square-root branch is fixed by the usual damped [Fresnel integral](../../../../../../fresnel-integral.md), or continuation from the Euclidean kernel. The hint's $dq'/\sqrt{\Delta t}$ contains the essential time-step dependence; the constant $(2\pi i)^{-1/2}$ fixes the identity limit and is included at every step.

Put $\eta=q'-q$. The normalized oscillatory Gaussian has moments

$$
\langle1\rangle=1,\qquad\langle\eta\rangle=0,\qquad\langle\eta^2\rangle=i\Delta t,\qquad\langle\eta^4\rangle=3(i\Delta t)^2.
$$

Taylor-expand the smooth [wavefunction](../../../../../../wave-function.md) and the potential over one short step. Odd moments vanish, and potential-derivative corrections first contribute at order $(\Delta t)^2$. Thus

$$
\psi(q,t+\Delta t)=\psi(q,t)+\frac{i\Delta t}{2}\partial_q^2\psi(q,t)-i\Delta t V(q)\psi(q,t)+O((\Delta t)^2).
$$

Subtract the initial value, divide by $\Delta t$ and take the limit:

$$
\boxed{i\partial_t\psi(q,t)=\left[-\frac12\partial_q^2+V(q)\right]\psi(q,t).}
$$

This proves the [Time-dependent Schrödinger equation](../../../../../../time-dependent-schrodinger-equation.md) by the [Schrödinger equation from a short-time path integral](../../../../../../schrodinger-equation-from-a-short-time-path-integral.md) argument. Nonuniform partitions give the same limit when their largest time step tends to zero.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
