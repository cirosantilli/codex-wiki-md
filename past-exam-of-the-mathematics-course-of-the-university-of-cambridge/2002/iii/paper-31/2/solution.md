<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $g(x)=\log|x|$ on $\mathbb R^2\setminus\{0\}$,

$$
\nabla g(x)=\frac{x}{|x|^2},\qquad \Delta g(x)=0.
$$

The [Itô formula](../../../../../ito-s-lemma.md), stopped in a compact [annulus](../../../../../annulus-mathematics.md), therefore gives

$$
dM_t=\frac{B_t}{|B_t|^2}\mathbin\cdot dB_t.
$$

This proves the [local martingale](../../../../../local-martingale.md) property up to a possible hitting of the origin. For the [annulus](../../../../../annulus-mathematics.md) exit time $T$, $M_{t\wedge T}$ is bounded between $\log r$ and $\log R$, so it is a true [uniformly integrable martingale](../../../../../uniformly-integrable-martingale.md).

The exit is finite almost surely. Indeed $|B_t|^2-2t$ is a [martingale](../../../../../martingale-split.md), so stopping at $T\wedge t$ gives $2\mathbb E(T\wedge t)=\mathbb E|B_{T\wedge t}|^2-1\le R^2-1$. Letting $t\to\infty$ proves $\mathbb ET<\infty$. Bounded convergence in the logarithmic [martingale](../../../../../martingale-split.md) now yields

$$
\boxed{\mathbb E M_T=M_0=0.}
$$

If $p$ is the [probability](../../../../../probability.md) of reaching radius $r$ before radius $R$, [continuity](../../../../../continuous-function.md) gives

$$
p\log r+(1-p)\log R=0,\qquad \boxed{p=\frac{\log R}{\log(R/r)}}.
$$

Hitting zero before reaching radius $R$ would require reaching every positive radius $r$ first. Its [probability](../../../../../probability.md) is bounded by $p$, which tends to zero as $r\downarrow0$. Any finite-time path hitting zero is bounded before that time and hence hits zero before exiting some integer-radius disk. A countable union over those disks proves **$B_t\ne0$ for every $t\ge0$, almost surely**. This is [planar Brownian motion avoids a fixed point](../../../../../planar-brownian-motion-avoids-a-fixed-point.md); it also makes $M$ a globally defined [continuous local martingale](../../../../../continuous-local-martingale.md).

To decide whether it is a true [martingale](../../../../../martingale-split.md), compute its [expectation](../../../../../expected-value.md) directly. Condition on $B_0$ if necessary and use rotation to take $B_0=(1,0)$ and write $B_t=B_0+W_t$. Conditional on $\rho=|W_t|$, the angle of $W_t$ is uniform. The [angular average of a logarithmic potential](../../../../../angular-average-of-a-logarithmic-potential.md) is

$$
\frac1{2\pi}\int_0^{2\pi}\log|1+\rho e^{i\theta}|d\theta=\log\max(1,\rho).
$$

For $\rho<1$ this follows by taking the real part of the convergent [power series](../../../../../power-series.md) for $\log(1+\rho e^{i\theta})$: each nonconstant Fourier term integrates to zero. For $\rho>1$ factor out $\rho$ and apply the same argument to $1/\rho$. The equality at one follows by the [integrable](../../../../../integrability.md) limiting logarithmic singularity. All interchanges are valid: the shifted [Gaussian density](../../../../../multivariate-normal-density.md) is bounded near the origin, where $\int_0^1r|\log r|dr<\infty$, and its [Gaussian](../../../../../normal-distribution.md) tail controls logarithmic growth.

The radius $\rho$ has density $(\rho/t)e^{-\rho^2/(2t)}$. Consequently, for $t>0$,

$$
\boxed{\mathbb E M_t=\int_1^\infty\log\rho\,\frac{\rho}{t}e^{-\rho^2/(2t)}d\rho=\int_1^\infty\frac{e^{-\rho^2/(2t)}}{\rho}d\rho>0.}
$$

Since $M_0=0$, **$M$ is not a [martingale](../../../../../martingale-split.md)**, despite [integrability](../../../../../integrability.md) at each deterministic time. This is the [logarithmic radius of planar Brownian motion](../../../../../logarithmic-radius-of-planar-brownian-motion.md) example.

The optional hint is consistent with this conclusion. The upper-radius exit $T(2,0)$ is finite and never occurs at zero. After that exit the stopped square is $(\log2)^2$; before it, a radius in $[1/2,2]$ also gives a logarithmic square no larger than $(\log2)^2$, while a radius below $1/2$ contributes precisely the extra indicated term. This proves the hinted inequality without assuming that the unstopped process is a true [martingale](../../../../../martingale-split.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
