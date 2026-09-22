<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a dense lower layer and write $g'=g(\rho_1-\rho_0)/\rho_0>0$. In the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) the fractional density difference is small; use the reference density in inertia and retain the difference in [buoyancy](../../../../../../buoyancy.md). The one-layer model additionally treats the ambient as much deeper, with negligible distributed horizontal inertia away from the head. The [shallow water](../../../../../../shallow-water-approximation.md) approximation requires depth small relative to the horizontal variation length, small vertical accelerations, nearly [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), and an approximately depth-uniform horizontal [velocity](../../../../../../velocity.md). Neglect mixing, [viscosity](../../../../../../dynamic-viscosity.md), bed friction and rotation. A slowly varying rectangular channel allows cross-sectional averages without large lateral separation.

A slice of width $b(x)$ contains volume $bh\,dx$. Its outgoing [volume flux](../../../../../../volumetric-flow-rate.md) is $bhu$, so [volume conservation](../../../../../../volume-conservation.md) gives $(bh)_t+(bhu)_x=0$. The integrated hydrostatic excess [pressure](../../../../../../pressure.md) is $\rho_0g'bh^2/2$. Pressure on the sloping side walls contributes $\rho_0g'h^2b'/2$ to the longitudinal force. The conservative [momentum](../../../../../../momentum.md) equation is therefore

$$
(bhu)_t+\left[bhu^2+\frac12g'bh^2\right]_x=\frac12g'h^2b'.
$$

Use the volume equation to simplify it. The resulting [shallow water equations](../../../../../../shallow-water-equations.md) are

$$
\boxed{h_t+uh_x+hu_x=-hu\frac{b'}b,\qquad u_t+uu_x+g'h_x=0.}
$$

Omitting the wall force would incorrectly introduce a width term into the material acceleration equation.

For $(h,u)$ the principal matrix is $\begin{pmatrix}u&h\\g'&u\end{pmatrix}$. Its [eigenvalues](../../../../../../eigenvalue.md) are $u\pm c$, where $c=\sqrt{g'h}$. For $h>0$ they are real and distinct, so the system is strictly [hyperbolic](../../../../../../hyperbolic-equilibrium-point.md). It degenerates at a dry front. From the volume equation, $c_t+uc_x+(c/2)u_x=-(cu/2)b'/b$. Combine this with the momentum equation to obtain the [variable-width shallow-water characteristics](../../../../../../variable-width-shallow-water-characteristics.md):

$$
\boxed{\frac{dx_\pm}{dt}=u\pm c,\qquad
\frac{d}{dt}(u\pm2c)\bigg|_{x_\pm(t)}=\mp cu\frac{b'}b.}
$$

In a constant-width channel $u\pm2c$ are [Riemann invariants](../../../../../../riemann-invariant.md) along the corresponding [characteristic curves](../../../../../../characteristic-curve.md); with varying width they satisfy compatibility equations with a source term.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
