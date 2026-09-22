<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Neglect the [inertia](../../../../inertia.md) of the [sphere](../../../../sphere.md) and balance the applied [force](../../../../force-split.md) against [Stokes drag](../../../../stokes-s-law.md). The [sphere](../../../../sphere.md) translates with $\mathbf U=\mathbf F_1/\zeta$, where $\zeta=6\pi\mu a$. The applied [force](../../../../force-split.md) is also the net [force](../../../../force-split.md) transmitted to the fluid; the fluid's drag on the [sphere](../../../../sphere.md) has the opposite sign.

Translate the origin to $\mathbf r_1$. In the solution of part [a](../a.md), retain the terms of order $a/r$ and discard those of order $a^3/r^3$. With $\mathbf n=(\mathbf x-\mathbf r_1)/r$,

$$
\begin{aligned}
\mathbf u(\mathbf x)
&\sim\frac{3a}{4r}(I+\mathbf n\mathbf n^T)\mathbf U\\
&=\boxed{\frac1{8\pi\mu r}(I+\mathbf n\mathbf n^T)\mathbf F_1}.
\end{aligned}
$$

This is the [Stokeslet](../../../../stokeslet.md), or equivalently the [Oseen tensor](../../../../oseen-tensor.md) $\mathsf G(\mathbf r)=(I+\mathbf n\mathbf n^T)/(8\pi\mu r)$ acting on $\mathbf F_1$. The omitted finite-size [velocity](../../../../velocity.md) is of order $a^2|\mathbf F_1|/(\mu r^3)$, so the displayed term is the leading far field for $r\gg a$. The singular [Stokeslet](../../../../stokeslet.md) must not be evaluated at its own centre to obtain a particle's self mobility.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
