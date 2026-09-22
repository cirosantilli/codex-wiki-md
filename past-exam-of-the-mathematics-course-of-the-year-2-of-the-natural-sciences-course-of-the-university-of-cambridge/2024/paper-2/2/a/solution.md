<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [harmonic extension in a circular sector](../../../../../harmonic-extension-in-a-circular-sector.md), write a separated [harmonic function](../../../../../harmonic-function.md) as $F(r)H(\theta)$. The [Laplace equation in polar coordinates](../../../../../laplace-equation-in-polar-coordinates.md) yields

$$
\frac{r(rF')'}{F}=-\frac{H''}{H}=\nu^2.
$$

The angular [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) select the [Fourier sine basis](../../../../../fourier-sine-basis.md)

$$
H_n(\theta)=\sin\frac{n\theta}{2\alpha},\qquad \nu_n=\frac{n}{2\alpha},\quad n=1,2,\ldots.
$$

Indeed, the angular equation has no nonzero solution with nonpositive $\nu^2$: multiplying $-H''=\nu^2H$ by $H$ and integrating gives $\int(H')^2=\nu^2\int H^2$. The radial [Cauchy-Euler equation](../../../../../cauchy-euler-equation.md) has solutions $r^{\nu_n}$ and $r^{-\nu_n}$. Boundedness at the vertex excludes the latter, so [superposition](../../../../../superposition-principle.md) gives

$$
\boxed{\Phi(r,\theta)=\sum_{n=1}^\infty A_n r^{n/(2\alpha)}\sin\frac{n\theta}{2\alpha}.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
