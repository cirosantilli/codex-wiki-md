<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The one-sided [Laplace transform](../../../../laplace-transform.md) is $\bar f(p)=\int_0^\infty e^{-pt}f(t)dt$. Its [Bromwich inversion formula](../../../../bromwich-inversion-formula.md) is $f(t)=(2\pi i)^{-1}\int_{\gamma-i\infty}^{\gamma+i\infty}e^{pt}\bar f(p)dp$, with an upward vertical contour to the right of all singularities and within the appropriate convergence half-plane.

To derive the [convolution theorem for Laplace transforms](../../../../convolution-theorem-for-laplace-transforms.md), transform $x(t)=\int_0^tf(\tau)g(t-\tau)d\tau$. With $u=t-\tau\geq0$, the triangular integration region becomes a quadrant. [Fubini's theorem](../../../../fubini-s-theorem.md) gives $\bar x(p)=\int_0^\infty\int_0^\infty e^{-p(u+\tau)}f(\tau)g(u)du\,d\tau=\bar f(p)\bar g(p)$, under the usual absolute convergence hypotheses. Inversion gives the required convolution formula.

For the differential equation, the transformed initial conditions give $(p^2-1)\bar y=\bar g+p+1$, hence $\bar y=\bar g/(p^2-1)+1/(p-1)$. Since $\mathcal L[\sinh t]=1/(p^2-1)$ for $\operatorname{Re}p>1$, the convolution yields

$$
\boxed{y(t)=e^t+\int_0^t\sinh(t-\tau)g(\tau)d\tau.}
$$

The integral and its first derivative vanish at zero, so the homogeneous term supplies both initial values. Differentiating twice gives the forcing through the unit derivative of the hyperbolic-sine kernel at zero.

## ↑ Ancestors (12)

1. [5](../5.md)
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
