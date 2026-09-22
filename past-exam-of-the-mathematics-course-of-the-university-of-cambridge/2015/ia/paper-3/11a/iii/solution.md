<h1 id="11a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\mathbf x=r\boldsymbol\omega$, with $|\boldsymbol\omega|=1$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) in [spherical coordinates](../../../../../../spherical-coordinate-system.md) gives $dS=r^2d\omega=r^2\sin\theta\,d\theta\,d\varphi$, so

$$
f(r)=\frac1{4\pi}\int_{S^2}\phi(r\boldsymbol\omega)\,d\omega.
$$

Differentiation under this fixed-domain integral yields

$$
f'(r)=\frac1{4\pi}\int_{S^2}\nabla\phi(r\boldsymbol\omega)\cdot\boldsymbol\omega\,d\omega
=\frac1{4\pi r^2}\int_{\partial V_r}\frac{\partial\phi}{\partial n}\,dS
=\frac1{4\pi r^2}\int_{V_r}\nabla^2\phi\,dV=0.
$$

The last step is the [divergence theorem](../../../../../../divergence-theorem.md) and the [Laplace equation](../../../../../../laplace-equation.md). Hence $f$ is constant on radii for which the closed ball lies inside $V$. Continuity at the origin gives $\lim_{r\to0}f(r)=\phi(0)$, proving the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md):

$$
\boxed{f(r)=\phi(0).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
