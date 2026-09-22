<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the observation point $\mathbf x$ and apply [Green's second identity](../../../../../green-second-identity.md) in the source variable $\mathbf y$. Since $\Delta u=0$, $\Delta_{\mathbf y}G_D=\delta_{\mathbf x}$ and $G_D=0$ on the boundary, it gives

$$
u(\mathbf x)=\int_D(u\Delta G_D-G_D\Delta u)\,d^2y
=\int_{\partial D}f(\mathbf y)\partial_{n_{\mathbf y}}G_D(\mathbf x,\mathbf y)\,ds_{\mathbf y}.
$$

The identity can be justified by deleting a small circle about $\mathbf x$ and letting its radius tend to zero; the logarithmic flux contributes $u(\mathbf x)$.

Set $\mathbf x=(r,\phi)$ and $\mathbf y=(\rho,\phi')$, and write $c=\cos(\phi-\phi')$. The symmetric expression for the [Green's function](../../../../../green-s-function-split.md) is

$$
G_D=\frac1{4\pi}\log\frac{r^2+\rho^2-2r\rho c}{1+r^2\rho^2-2r\rho c}.
$$

At the boundary, the outward [normal derivative](../../../../../normal-derivative.md) is $\partial_\rho$ at $\rho=1$, and hence

$$
\left.\partial_\rho G_D\right|_{\rho=1}
=\frac1{4\pi}\frac{(2-2rc)-(2r^2-2rc)}{1+r^2-2rc}
=\frac1{2\pi}\frac{1-r^2}{1-2rc+r^2}.
$$

Since $ds=d\phi'$ on the [unit circle](../../../../../complex-unit-circle.md), the [Poisson integral on the unit disk](../../../../../poisson-integral-on-the-unit-disk.md) follows, with [Poisson kernel](../../../../../poisson-kernel.md)

$$
\boxed{P(r,\vartheta)=\frac{1-r^2}{1-2r\cos\vartheta+r^2}},\qquad
u(r,\phi)=\frac1{2\pi}\int_0^{2\pi}f(\phi')P(r,\phi-\phi')\,d\phi'.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
