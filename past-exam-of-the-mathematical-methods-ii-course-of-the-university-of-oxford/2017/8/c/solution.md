<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The boundary consists of the spherical zone $-a\le z\le a$ and the inner cylindrical wall. On the sphere, $n=r/R$, so $n\cdot r=R$. Its area element is $R\,d\phi\,dz$, giving the flux

$$
\int_{-a}^{a}\int_0^{2\pi}R^2\,d\phi\,dz=4\pi aR^2.
$$

On the inner cylinder, the outward normal of the remaining material points _towards the hole_: $n=-e_\rho$. Therefore $n\cdot r=-r_0$, and $dS=r_0\,d\phi\,dz$, giving flux $-4\pi ar_0^2$. There are no planar end faces of positive area: the two surfaces meet along the rim circles. Hence

$$
\boxed{V=\frac{4\pi a}{3}(R^2-r_0^2)
=\frac{4\pi a^3}{3}=\frac{\pi h^3}{6}.}
$$

Using the cylinder's radial normal with the opposite sign would count the hole as extra material and lose the required cancellation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
