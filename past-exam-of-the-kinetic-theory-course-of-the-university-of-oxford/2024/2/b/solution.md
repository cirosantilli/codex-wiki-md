<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A linearly stable $f_0$ has no zeros of the causal [dielectric function](../../../../dielectric-function.md) in $\operatorname{Re}p>0$. Hence the inverse [Laplace transform](../../../../laplace-transform.md) contours can approach $\sigma=0^+$, retaining the causal boundary value at $p=-i\omega+0^+$. To obtain a stationary forced response, further assume that the excited collective perturbations actually damp. This is the decay condition in the question's long-time instruction.

A transparent evaluation of the double integral uses the stationary [power spectral density](../../../../power-spectral-density.md). The [white noise](../../../../white-noise.md) covariance $2A_k\delta(t-t')$ has temporal spectrum $2A_k$. Linear filtering by $1/\epsilon$ therefore gives

$$
S_{\varphi,k}(\omega)=\frac{2A_k}{|\epsilon(-i\omega+0^+,k)|^2},\qquad
\langle\varphi_k(t-\tau)\varphi_k(t)^*\rangle=\int_{-\infty}^{\infty}\frac{d\omega}{2\pi}\,S_{\varphi,k}(\omega)e^{i\omega\tau}.
$$

The causal solution for $\delta f_k$ in [a](../a.md) gives, after the initial transients have decayed,

$$
D(v)=\frac{e^2}{m_e^2}\sum_k k^2\operatorname{Re}\int_0^\infty d\tau\,e^{-ikv\tau}\langle\varphi_k(t-\tau)\varphi_k(t)^*\rangle.
$$

The real part can be taken because the full $k$ sum pairs conjugates. Using the [distribution theory](../../../../distribution-theory-split.md) identity $\operatorname{Re}\int_0^\infty e^{ia\tau}\,d\tau=\pi\delta(a)$, with a positive vanishing convergence factor, samples the temporal spectrum at $\omega=kv$:

$$
\boxed{D(v)=\frac{e^2}{m_e^2}\sum_k\frac{k^2A_k}{|\epsilon(-ikv+0^+,k)|^2}.}
$$

The factor $1/2$ from the one-sided time integral cancels the $2$ in the noise covariance. The result is nonnegative, as a stationary [velocity-space diffusion](../../../../velocity-space-diffusion.md) coefficient should be.

**Qualification of stability.** Absence of growing modes alone does not guarantee this stationary limit. For example, the electron [waterbag distribution](../../../../waterbag-distribution.md) $f_0(v)=n_e\mathbf1_{|v|<V}/(2V)$ has

$$
\epsilon(-i\omega,k)=1-\frac{\omega_{pe}^2}{\omega^2-k^2V^2},\qquad \omega^2=k^2V^2+\omega_{pe}^2
$$

as undamped collective roots. [White noise](../../../../white-noise.md) drives their field variance to grow instead of settling. Thus the formula requires decay of excited modes, not merely absence of exponentially growing ones. For weak [Landau damping](../../../../landau-damping.md), the waiting time can be much longer than $\omega_{pe}^{-1}$, and must still be short compared with evolution of $f_0$ for the frozen-background [quasilinear approximation](../../../../quasilinear-approximation.md) to apply.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
