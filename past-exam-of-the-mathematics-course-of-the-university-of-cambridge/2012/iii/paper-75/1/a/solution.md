<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For two incompressible [Stokes flows](../../../../../../stokes-flow-split.md) $(\mathbf u,\boldsymbol\sigma)$ and $(\widehat{\mathbf u},\widehat{\boldsymbol\sigma})$ with the same viscosity and no body forces, the [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) states

$$
\int_{\partial D}\mathbf u\cdot\widehat{\boldsymbol\sigma}\mathbf n\,dS
=\int_{\partial D}\widehat{\mathbf u}\cdot\boldsymbol\sigma\mathbf n\,dS.
$$

Indeed the divergence of their difference is zero: stress divergences vanish, pressure contracts with zero velocity divergence, and the two symmetric strain-rate contractions cancel.

Apply it to the decaying disturbance $\mathbf u'=\mathbf u-\mathbf u_\infty$ around the sphere and an auxiliary translating sphere of velocity $\mathbf V$. On the body surface, $\mathbf u'=\mathbf U+\boldsymbol\Omega_s\times\mathbf x-\mathbf u_\infty$. Using normals from the body into the fluid, the given auxiliary traction is $-3\mu\mathbf V/(2a)$; reversing both normal conventions does not change the reciprocal equality. The background traction integrates to zero because it is regular inside the sphere. The disturbance's hydrodynamic force is consequently $\mathbf F_H=-\mathbf F$, where $\mathbf F$ is the externally applied force. The rotational term integrates to zero. Thus for arbitrary $\mathbf V$,

$$
-\frac{3\mu}{2a}\mathbf V\cdot\left(4\pi a^2\mathbf U-\int_{S_a}\mathbf u_\infty\,dS\right)
=-\mathbf V\cdot\mathbf F.
$$

Therefore $\mathbf U=\mathbf F/(6\pi\mu a)+\langle\mathbf u_\infty\rangle_{S_a}$.

The background Stokes equations imply $\nabla^2p_\infty=0$ and $\nabla^4\mathbf u_\infty=0$. The [spherical mean of a biharmonic function](../../../../../../spherical-mean-of-a-biharmonic-function.md) gives exactly $\langle\mathbf u_\infty\rangle=\mathbf u_\infty+(a^2/6)\nabla^2\mathbf u_\infty$, evaluated at the sphere center. One can obtain it from Taylor expansion and $\langle x_ix_j\rangle=a^2\delta_{ij}/3$; every subsequent spherical average contains $\nabla^4$ and vanishes. This requires the background to be regular throughout the enclosed ball. **Hence the [Faxén relation](../../../../../../faxen-s-first-law.md) is**

$$
\boxed{\mathbf U=\frac{\mathbf F}{6\pi\mu a}+
\left(1+\frac{a^2}{6}\nabla^2\right)\mathbf u_\infty\bigg|_{\mathbf x=\mathbf x_c}.}
$$

The printed denominator $6\pi\mu$ omits $a$. The given traction integrates to $-6\pi\mu a\mathbf V$, fixing that factor; the printed force term also fails dimensional consistency unless its force were redefined, which the question does not do.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
