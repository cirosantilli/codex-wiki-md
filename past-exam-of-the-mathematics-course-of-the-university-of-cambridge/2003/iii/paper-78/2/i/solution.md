<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $u(x,z,t)$ be displacement along the source line and let $F(t)$ be its force per unit length. The [shear-horizontal wave](../../../../../../shear-horizontal-wave.md) equation is

$$
\rho u_{tt}-\mu\Delta u=F(t)\delta^{(2)}(x,z),\qquad \mu=\rho\beta^2.
$$

Rotational symmetry about the line makes $u=u(r,t)$. Integrate over a disk of radius $r$ and use the [divergence theorem](../../../../../../divergence-theorem.md):

$$
\rho\int_{D_r}u_{tt}\,dA-2\pi\mu r u_r=F(t).
$$

At a fixed regular time, a logarithmic singularity and its time derivatives are locally integrable; the inertial integral is $O(r^2|\log r|)$ and vanishes as $r\downarrow0$. The leading balance is consequently $r u_r=-F(t)/(2\pi\mu)$, giving the [SH line-source near-field singularity](../../../../../../sh-line-source-near-field-singularity.md)

$$
\boxed{u(r,t)=-\frac{F(t)}{2\pi\mu}\log\frac r{r_*}+O(1)\qquad(r\downarrow0)}.
$$

The reference length $r_*$ only changes the bounded term; boundary conditions and source history determine that term. This is a local fixed-time statement, interpreted distributionally in time if the source force has jumps. It establishes logarithmic spatial dependence directly, without extrapolating far-field ray spreading into the source.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
