<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a separated weighted density, write $P_n=e^{\gamma t}p(\sigma)$. Its [eigenvalue equation](../../../../../../eigenvalue-equation.md) is

$$
\frac\kappa2p''+\frac1\tau(\sigma p)'+n\sigma p=\gamma p.
$$

Set $p=\psi\exp[-\sigma^2/(2\kappa\tau)]$. Differentiation eliminates the first derivative of $\psi$, giving the [tilted Ornstein-Uhlenbeck oscillator transformation](../../../../../../tilted-ornstein-uhlenbeck-oscillator-transformation.md)

$$
\frac\kappa2\psi''+\left[\frac1{2\tau}-\frac{\sigma^2}{2\kappa\tau^2}+n\sigma\right]\psi=\gamma\psi.
$$

Complete the square and introduce the [dimensionless variable](../../../../../../dimensionless-variable.md) $x=(\sigma-\kappa n\tau^2)/\sqrt{\kappa\tau}$. The equation becomes

$$
\frac{d^2\psi}{dx^2}+\left[1+\kappa n^2\tau^3-2\gamma\tau-x^2\right]\psi=0.
$$

Comparing with the [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator.md) gives $2E=1+\kappa n^2\tau^3-2\gamma\tau$. Its energies $E_m=m+1/2$ therefore correspond to $\gamma_m=\kappa n^2\tau^2/2-m/\tau$. The dominant nonnegative separated mode is the [ground state](../../../../../../ground-state.md), which is [nodeless](../../../../../../nodeless-eigenfunction.md). Consequently

$$
\boxed{\gamma_n=\frac12\kappa\tau^2n^2.}
$$

For an independent check, $\log[\widetilde B(t)/B_0]=\int_0^t\widetilde\sigma(s)\,ds$ is a centered [Gaussian random variable](../../../../../../gaussian-random-variable.md) with [variance](../../../../../../variance-split.md)

$$
V(t)=\kappa\tau^2\left[t-2\tau(1-e^{-t/\tau})+\frac\tau2(1-e^{-2t/\tau})\right].
$$

The [exponential moment of a Gaussian linear functional](../../../../../../exponential-moment-of-a-gaussian-linear-functional.md) gives $\mathbb E[B^n]=B_0^n\exp[n^2V(t)/2]$, whose long-time growth rate is the same $\gamma_n$. This exact [Ornstein-Uhlenbeck multiplicative amplification](../../../../../../ornstein-uhlenbeck-multiplicative-amplification.md) formula also distinguishes the finite-time transient from the asymptotic exponential law. A general transient can contain sign-changing excited eigenfunctions in its expansion while the total weighted density remains nonnegative.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
