<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [Keplerian accretion disk](../../../../../../keplerian-accretion-disk.md), $\Omega=(GM_{\rm BH}/R^3)^{1/2}$, so

$$
F(R)=\frac{9GM_{\rm BH}}{4R^3}\nu\Sigma
=\frac{3GM_{\rm BH}\dot m}{4\pi R^3}
\left[1-\left(\frac{R_{\rm ISCO}}R\right)^{1/2}\right].
$$

Here $F$ is the dissipation summed over the two faces. The total luminosity is

$$
L=\int_{R_{\rm ISCO}}^\infty2\pi R F(R)\,dR
=\boxed{\frac{GM_{\rm BH}\dot m}{2R_{\rm ISCO}}}.
$$

This is the [binding energy](../../../../../../newtonian-gravitational-potential-energy.md) per unit mass of a circular orbit at the inner edge, multiplied by the accretion rate. The [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md) ensures that no additional mechanical work enters from smaller radii.

The luminosity emitted outside radius $R$ is

$$
L(>R)=\frac{3GM_{\rm BH}\dot m}{2R}
\left[1-\frac23\left(\frac{R_{\rm ISCO}}R\right)^{1/2}\right].
$$

Writing $y=(R_{\rm ISCO}/R)^{1/2}$, the condition $L(>R)=L/2$ becomes $3y^2-2y^3=1/2$. Its physical root is $y=1/2$, and hence

$$
\boxed{R_{1/2}=4R_{\rm ISCO}}.
$$

Half of a thin disk's luminosity therefore comes from only the innermost factor four in radius, so strong-gravity effects and the inner-boundary condition strongly influence its observed spectrum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
