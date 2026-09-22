<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose the [Green function](../../../../green-s-function-split.md) convention $\Delta_{\mathbf r}G(\mathbf r;\mathbf r_0)=\delta^{(3)}(\mathbf r-\mathbf r_0)$, with decay at infinity and no extra singularities. For sufficiently decaying source data,

$$
\boxed{\Phi(\mathbf r_0)=\int_{\mathbb R^3}G(\mathbf r;\mathbf r_0)\sigma(\mathbf r)\,d^3r,\qquad G=-\frac1{4\pi|\mathbf r-\mathbf r_0|}.}
$$

Away from its source, this [fundamental solution of the Laplace equation](../../../../fundamental-solution-of-the-laplace-equation.md) is harmonic. Its radial derivative is $1/(4\pi\rho^2)$, so the flux of its [gradient](../../../../gradient.md) through a small source-centred sphere is one. The [divergence theorem](../../../../divergence-theorem.md) therefore supplies exactly the unit [Dirac delta function](../../../../dirac-delta-function.md) required by the equation. Decay at infinity excludes an added globally regular harmonic term.

For the half-space, reflect the source to $\mathbf r_0^*=(-x_0,y_0,z_0)$. The [method of images](../../../../method-of-images.md) gives the zero-boundary [Dirichlet Green function](../../../../dirichlet-green-function.md)

$$
\widetilde G=-\frac1{4\pi}\left(\frac1{|\mathbf r-\mathbf r_0|}-\frac1{|\mathbf r-\mathbf r_0^*|}\right).
$$

The two distances coincide at $x=0$, and also cancel if the source lies on the plane. The image singularity lies outside the physical domain.

The [sign conventions for a Dirichlet Green function](../../../../sign-conventions-for-a-dirichlet-green-function.md) require care here. With $\Delta\widetilde G=+\delta$, [Green's second identity](../../../../green-second-identity.md) gives $\Phi(\mathbf r_0)=\int_{\partial\Omega}f\,\partial_n\widetilde G\,dS$. At this wall the outward normal is $-\mathbf e_x$, so $\partial_n\widetilde G=-\partial_x\widetilde G$. Direct differentiation gives $\partial_x\widetilde G|_{x=0}=-x_0/(2\pi d^3)$, where $d^2=x_0^2+(y-y_0)^2+(z-z_0)^2$. Thus the printed intermediate formula with $+\partial_x\widetilde G$ needs a minus sign for its stated Green convention. The final [Poisson kernel for the upper half-space](../../../../poisson-kernel-for-the-upper-half-space.md) is positive:

$$
\boxed{\Phi(\mathbf r_0)=\frac{x_0}{2\pi}\int_{\mathbb R^2}\frac{f(y,z)\,dy\,dz}{[x_0^2+(y-y_0)^2+(z-z_0)^2]^{3/2}}.}
$$

Its boundary integral is one for constant data, providing an independent sign check.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
