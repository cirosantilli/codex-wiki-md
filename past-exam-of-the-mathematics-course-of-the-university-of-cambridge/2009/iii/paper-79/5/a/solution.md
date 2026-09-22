<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\boldsymbol U=(u,v)$, $\zeta=v_x-u_y$ and $D/Dt=\partial_t+\boldsymbol U\cdot\nabla$. The inviscid [shallow water equations](../../../../../../shallow-water-equations.md) are

$$
\frac{D\boldsymbol U}{Dt}+f\hat{\boldsymbol z}\times\boldsymbol U=-g\nabla(h+H),\qquad \frac{Dh}{Dt}=-h\nabla\cdot\boldsymbol U.
$$

Taking the vertical curl of the momentum equation, with constant $f$, gives $D\zeta/Dt=-(f+\zeta)\nabla\cdot\boldsymbol U$. Combining this with the depth equation proves

$$
\boxed{P=\frac{f+\zeta}{h},\qquad \frac{DP}{Dt}=0.}
$$

Thus [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md) is materially conserved: changes in [absolute vorticity](../../../../../../absolute-vorticity.md) are exactly compensated by stretching or compression of the layer depth.

The relation to a [Bernoulli function](../../../../../../bernoulli-function.md) presupposes [steady flow](../../../../../../steady-flow.md). In that case define $B=g(h+H)+\tfrac12|\boldsymbol U|^2$. The vector identity $(\boldsymbol U\cdot\nabla)\boldsymbol U=\nabla(\tfrac12|\boldsymbol U|^2)+\zeta\hat{\boldsymbol z}\times\boldsymbol U$ gives

$$
\nabla B=-(f+\zeta)\hat{\boldsymbol z}\times\boldsymbol U.
$$

Steady [volume conservation](../../../../../../volume-conservation.md) allows a transport [stream function](../../../../../../stream-function.md) with $h\boldsymbol U=(\psi_y,-\psi_x)$. Hence $\hat{\boldsymbol z}\times(h\boldsymbol U)=\nabla\psi$, so

$$
\nabla B=-P\nabla\psi,\qquad \boxed{\frac{dB}{d\psi}=-P.}
$$

In particular, $\boldsymbol U\cdot\nabla B=0$: the [Bernoulli function](../../../../../../bernoulli-function.md) is constant along each [streamline](../../../../../../streamline.md). Where the flow permits a single-valued dependence on the [stream function](../../../../../../stream-function.md), the displayed derivative describes how that constant changes between neighbouring [streamlines](../../../../../../streamline.md). For an unsteady flow, [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md) remains conserved but the stated steady [Bernoulli function](../../../../../../bernoulli-function.md) relation does not generally hold.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
