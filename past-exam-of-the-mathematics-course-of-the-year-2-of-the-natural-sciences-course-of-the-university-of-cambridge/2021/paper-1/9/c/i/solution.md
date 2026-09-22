<h1 id="9/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On the cylindrical surface $r=R$, the [line element](../../../../../../line-element.md) is $ds^2=R^2d\theta^2+dz^2$. For a single-valued path parametrized by increasing $\theta$,

$$
\boxed{L[z]=\int_{\theta_1}^{\theta_2}\sqrt{R^2+z'^2}\,d\theta.}
$$

The integrand has no explicit $z$, so its [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) gives the constant conjugate quantity $z'/\sqrt{R^2+z'^2}$. Its [derivative](../../../../../../derivative.md) with respect to $z'$ is strictly positive, hence $z'$ itself is constant. The two endpoints determine

$$
\boxed{z(\theta)=z_1+\frac{z_2-z_1}{\pi}\left(\theta+\frac\pi2\right),\qquad-\frac\pi2\leq\theta\leq\frac\pi2.}
$$

This is a constant-pitch [helix](../../../../../../helix.md) on the cylinder. To verify global minimality, unroll the cylinder with planar coordinates $(R\theta,z)$. The path becomes a straight line between points separated by $\pi R$ and $z_2-z_1$, so the [triangle inequality](../../../../../../triangle-inequality.md) for arc length gives

$$
\boxed{L_{\min}=\sqrt{\pi^2R^2+(z_2-z_1)^2}.}
$$

This is the standard description of [geodesics on a circular cylinder](../../../../../../geodesics-on-a-circular-cylinder.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
