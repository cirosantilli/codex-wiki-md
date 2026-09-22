<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $q=|r-r'|$. Away from the source, the radial [Laplacian](../../../../../laplacian.md) gives $\nabla^2(-1/(4\pi q))=q^{-2}\partial_q[q^2/(4\pi q^2)]=0$. Through a small source-centred sphere, the outward flux of its gradient is

$$
\int_{q=\varepsilon}\partial_qH\,dS=\frac{1}{4\pi\varepsilon^2}4\pi\varepsilon^2=1.
$$

This identifies a unit [Dirac delta](../../../../../dirac-delta-function.md) at the source. More explicitly, for a smooth compactly supported test function $\psi$, apply [Green's second identity](../../../../../green-second-identity.md) outside the radius-$\varepsilon$ ball. The inner outward normal of that punctured domain is $-e_q$. The term $H\partial_n\psi$ has integral $O(\varepsilon)$, while $-\psi\partial_nH$ tends to $\psi(r')$. Thus $\int H\nabla^2\psi\,dV=\psi(r')$, proving the distributional identity

$$
\boxed{\nabla^2H(r,r')=\delta^{(3)}(r-r').}
$$

Whenever the integral converges, convolution with this [Green function of the Laplacian](../../../../../green-function-of-the-laplacian.md) solves the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md):

$$
\boxed{\Phi(r)=-G\int_{\mathbb R^3}\frac{\rho(r')}{|r-r'|}\,d^3r'+h(r),\qquad\nabla^2h=0.}
$$

The harmonic term represents the homogeneous freedom and is fixed by boundary conditions. For an isolated finite mass distribution, regularity away from the prescribed sources and the normalization $\Phi\to0$ at infinity select $h=0$.

For a point mass at the origin, the delta integral gives the [Newtonian potential of a point mass](../../../../../newtonian-potential-of-a-point-mass.md),

$$
\boxed{\Phi(r)=-\frac{GM}{|r|},\qquad r\ne0,\qquad\Phi(\infty)=0.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
