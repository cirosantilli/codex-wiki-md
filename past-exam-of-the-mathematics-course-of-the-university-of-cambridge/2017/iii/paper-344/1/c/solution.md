<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With periodic or sufficiently decaying [boundary conditions](../../../../../../boundary-condition.md), [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\frac{\delta F}{\delta\phi}=a\phi-\kappa\nabla^2\phi.
$$

Assume $\kappa\ge0$ for a stable quadratic [free energy](../../../../../../thermodynamic-free-energy.md); the diffusive smoothing discussed below requires $\kappa>0$. In a periodic box of volume $V$, use the unitary convention $\phi_{\mathbf q}=V^{-1/2}\int_V\phi(\mathbf r)e^{-i\mathbf q\cdot\mathbf r}\,d\mathbf r$. A real field has $\phi_{-\mathbf q}=\phi_{\mathbf q}^*$. Since the [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) converts $\nabla^2$ to $-q^2$, each [Fourier mode](../../../../../../fourier-mode.md) obeys

$$
\boxed{\dot\phi_{\mathbf q}=-r(q)\phi_{\mathbf q}+\eta_{\mathbf q},\qquad r(q)=\Gamma(a+\kappa q^2)>0.}
$$

It is an [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md). Multiplication by the integrating factor $e^{r(q)t}$ gives

$$
\boxed{\phi_{\mathbf q}(t)=e^{-r(q)t}\phi_{\mathbf q}(0)+\int_0^t e^{-r(q)(t-s)}\eta_{\mathbf q}(s)\,ds.}
$$

The noise integral is understood as an [Itô integral](../../../../../../ito-integral.md) with a deterministic kernel; writing $\eta\,ds$ is shorthand for the corresponding Wiener increment. Direct differentiation in the mild stochastic sense checks both the equation and the initial value. The stated Kronecker-delta noise covariance corresponds to this finite-volume normalization. Unlike a [conserved order parameter](../../../../../../conserved-order-parameter.md), the zero [wavenumber](../../../../../../wavenumber.md) mode decays at the nonzero rate $\Gamma a$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
