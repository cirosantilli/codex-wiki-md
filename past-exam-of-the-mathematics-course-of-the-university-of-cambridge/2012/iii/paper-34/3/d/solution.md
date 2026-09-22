<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On a compact time interval a continuous path avoiding the origin has a strictly positive minimum radius. Thus the times $S_{1/n}$ tend to infinity almost surely. Part (a) localizes $M_t=\log|B_t|$, so $M$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md).

To show that it is not a [martingale](../../../../../../martingale-split.md), compute its [expectation](../../../../../../expected-value.md) at a positive deterministic time. In distribution $B_t=(1,0)+W_t$, where $W_t$ is a centered isotropic Gaussian vector. Conditional on $\rho=|W_t|$, its angle is uniform. The [angular average of a logarithmic potential](../../../../../../angular-average-of-a-logarithmic-potential.md) is

$$
\frac1{2\pi}\int_0^{2\pi}\log|1+\rho e^{i\theta}|\,d\theta=\log\max(1,\rho).
$$

For $\rho<1$ this follows by averaging the real part of the power series for $\log(1+\rho e^{i\theta})$; for $\rho>1$ factor out $\rho$ and apply the same argument to $\rho^{-1}$. The value at $1$ follows by the integrable logarithmic singularity, or is irrelevant for the continuously distributed radius.

The radius has density $(\rho/t)e^{-\rho^2/(2t)}$. The logarithm of $|B_t|$ is absolutely integrable: near the origin its Gaussian density is bounded and $\int_0^1r|\log r|\,dr<\infty$; away from the origin its positive part is bounded by a constant plus $|B_t|$. Therefore conditioning is legitimate, and integration by parts yields

$$
\boxed{\mathbb EM_t=\int_1^\infty\log\rho\,\frac\rho t e^{-\rho^2/(2t)}\,d\rho=\int_1^\infty\frac{e^{-\rho^2/(2t)}}\rho\,d\rho>0\quad(t>0).}
$$

Since $M_0=0$, this contradicts preservation of [expectation](../../../../../../expected-value.md) by a [martingale](../../../../../../martingale-split.md). Thus the [logarithmic radius of planar Brownian motion](../../../../../../logarithmic-radius-of-planar-brownian-motion.md) is a strict local [martingale](../../../../../../martingale-split.md). It is not a nonnegative local [martingale](../../../../../../martingale-split.md); its negative values allow its [expectation](../../../../../../expected-value.md) to increase.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
