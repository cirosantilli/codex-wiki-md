<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since the particle starts at the origin, its [Lagrangian trajectory](../../../../../../lagrangian-trajectory.md) satisfies $\boldsymbol X(t)=\int_0^t\boldsymbol v(s)ds$. Differentiating the mean-square displacement gives

$$
\frac{d}{dt}\langle|\boldsymbol X(t)|^2\rangle
=2\left\langle\boldsymbol v(t)\cdot\int_0^t\boldsymbol v(s)ds\right\rangle
=2\int_0^t\langle\boldsymbol v(t)\cdot\boldsymbol v(t-\tau)\rangle d\tau.
$$

Here we set $\tau=t-s$ and assume finite second moments so that averaging and integration commute. Under Lagrangian stationarity write the [autocorrelation](../../../../../../autocorrelation.md) as $R_L(\tau)$. Uniform fluid-tracer sampling in homogeneous incompressible turbulence gives $R_L(0)=\langle|\boldsymbol u|^2\rangle$. A second integration yields the exact [Taylor turbulent dispersion](../../../../../../taylor-turbulent-dispersion.md) formula

$$
\boxed{\langle|\boldsymbol X(t)|^2\rangle=2\int_0^t(t-\tau)R_L(\tau)d\tau.}
$$

For times short compared with [velocity](../../../../../../velocity.md) decorrelation, continuity at zero gives $R_L(\tau)\simeq R_L(0)$ throughout the integral. Thus

$$
\boxed{\langle|\boldsymbol X(t)|^2\rangle\simeq\langle|\boldsymbol u|^2\rangle t^2.}
$$

The particle retains nearly its initial [velocity](../../../../../../velocity.md): this is ballistic transport.

If $R_L$ is integrable, then at long times the displacement derivative approaches $2\int_0^\infty R_L(\tau)d\tau=2R_L(0)t_L$, using the [Lagrangian integral time](../../../../../../lagrangian-integral-time.md). Therefore

$$
\boxed{\langle|\boldsymbol X(t)|^2\rangle\sim2\langle|\boldsymbol u|^2\rangle t_Lt.}
$$

This is diffusive transport: successive long-time displacements lose memory of one another. In an isotropic three-dimensional [diffusion](../../../../../../diffusion.md) equation, $\langle X^2\rangle=6D_Tt$, so $D_T=\langle|\boldsymbol u|^2\rangle t_L/3$. The shorthand $t\ll t_L$ and $t\gg t_L$ presumes that $t_L$ is representative of the decorrelation time. With strongly oscillatory correlations, the area-based integral time need not characterize every crossover; the exact integral formula remains the appropriate starting point.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
