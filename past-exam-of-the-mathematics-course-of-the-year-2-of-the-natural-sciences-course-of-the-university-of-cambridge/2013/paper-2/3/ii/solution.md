<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the polar axis in the source integration along the evaluation vector $r$. The [Euclidean distance](../../../../../euclidean-distance.md) then satisfies $|r-r'|^2=r^2+r'^2-2rr'\cos\theta'$, giving

$$
H(r,r')=-\frac1{4\pi\sqrt{r^2+r'^2-2rr'\cos\theta'}}.
$$

For the uniform ball, integrate its [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) in these [spherical coordinates](../../../../../spherical-coordinate-system.md). With $\mu=\cos\theta'$,

$$
\Phi(r)=-2\pi G\rho\int_0^R r'^2dr'\int_{-1}^1\frac{d\mu}{\sqrt{r^2+r'^2-2rr'\mu}}.
$$

For $r,r'>0$, the inner integral is

$$
\frac{r+r'-|r-r'|}{rr'},
$$

obtained from the antiderivative $-\sqrt{r^2+r'^2-2rr'\mu}/(rr')$. Therefore

$$
\Phi(r)=-2\pi G\rho\int_0^R\frac{r'}r[r+r'-|r-r'|]dr'.
$$

For $0<r<R$, split the radial integral at $r'=r$. Its two pieces are $\int_0^r2r'^2dr'/r=2r^2/3$ and $\int_r^R2r'dr'=R^2-r^2$. The [Newtonian gravitational potential of a uniform solid sphere](../../../../../newtonian-gravitational-potential-of-a-uniform-solid-sphere.md) is consequently

$$
\boxed{\Phi(r)=-2\pi G\rho\left(R^2-\frac{r^2}{3}\right)=-\frac{GM}{2R^3}(3R^2-r^2),\quad 0\leq r<R,\qquad M=\frac{4\pi\rho R^3}{3}.}
$$

The centre value follows by continuity, removing the intermediate $1/r$. For $r>R$, the same integral gives $-GM/r$, so both the potential and first derivative match at the surface. Finally $\nabla^2\Phi=4\pi G\rho$ inside, while $-\nabla\Phi=-GM\mathbf r/R^3$ is directed inward and vanishes at the centre, checking the sign and normalization.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
