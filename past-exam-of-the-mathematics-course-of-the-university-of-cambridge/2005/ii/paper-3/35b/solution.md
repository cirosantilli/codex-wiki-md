<h1 id="35b/solution">Solution</h1>

↑ **Parent:** [35B](../35b.md)

Choose polar angle $\theta$ from the acceleration direction. Then $|n\times q\dot v|^2=q^2|\dot v|^2\sin^2\theta$. Integrating over the [solid angle](../../../../../solid-angle.md) gives $2\pi\int_0^\pi\sin^3\theta\,d\theta=8\pi/3$, and hence the specified normalization gives [Larmor formula](../../../../../larmor-formula.md)

$$
\boxed{P=\frac{\mu_0q^2}{6\pi}|\dot v|^2.}
$$

This uses the source's convention for radiated power; standard SI normalization has an additional factor $1/c$ in both given power formulas.

To leading order when $W\ll E$, neglect the loss while computing the head-on trajectory. Mechanical energy conservation gives $\tfrac12m\dot r^2+V(r)=E=V(r_0)$ and acceleration magnitude $|V'(r)|/m$. On each leg,

$$
dt=\sqrt{\frac m2}\frac{|dr|}{\sqrt{V(r_0)-V(r)}}.
$$

The incoming and outgoing legs contribute equally. Multiplying the power by this time element, adding both legs, and assuming the integral converges gives

$$
\boxed{W\simeq\frac{\mu_0q^2}{3\pi m^2}\sqrt{\frac m2}
\int_{r_0}^\infty\frac{[V'(r)]^2}{\sqrt{V(r_0)-V(r)}}\,dr.}
$$

Using the unperturbed turning point is justified at this order in the small radiative loss, for a regular turning trajectory.

## ↑ Ancestors (10)

1. [35B](../35b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
