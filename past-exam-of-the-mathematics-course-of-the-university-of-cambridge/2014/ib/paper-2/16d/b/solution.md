<h1 id="16d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Duhamel principle](../../../../../../duhamel-s-principle.md) superposes the response to source impulses:

$$
\boxed{\Psi(t,x,y)=\int_0^t
\frac{p(s)}{4\pi D(t-s)}
\exp\left[-\frac{x^2+y^2}{4D(t-s)}\right]ds.}
$$

This expression uses the source at the origin, is causal, and has zero initial data in the distributional sense. Its integral over the plane is $\int_0^tp(s)\,ds$, consistent with the injected total amount.

For the finite-duration source and $t>t_0$, set $b=(x^2+y^2)/(4D)$. The [causal diffusion from a finite-duration planar point source](../../../../../../causal-diffusion-from-a-finite-duration-planar-point-source.md) becomes

$$
\Psi=\frac{p_0}{4\pi D}\int_{t-t_0}^t\frac{e^{-b/\tau}}{\tau}\,d\tau.
$$

With $\eta=b/\tau$, or by differentiating the supplied [exponential integral](../../../../../../exponential-integral.md), this is

$$
\boxed{\Psi=\frac{p_0}{4\pi D}
\left[\operatorname{Ei}\left(-\frac b{t-t_0}\right)
-\operatorname{Ei}\left(-\frac bt\right)\right].}
$$

If $b/(t-t_0)\ll1$, both arguments are small. Their logarithmic constants and $\ln b$ cancel, leaving

$$
\boxed{\Psi(t,x,y)\approx\frac{p_0}{4\pi D}\ln\frac{t}{t-t_0}.}
$$

At the origin this logarithmic expression is exact for $t>t_0$, obtained as the limit $b\to0$. The leading spatial correction is $-p_0b\,t_0/[4\pi D\,t(t-t_0)]$. If also $t\gg t_0$, the leading value is $p_0t_0/(4\pi Dt)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16D](../../16d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
