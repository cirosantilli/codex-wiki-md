<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On the [unit circle](../../../../complex-unit-circle.md), put $z=e^{i\theta}$. Then $d\theta=dz/(iz)$ and $\cos\theta=(z+z^{-1})/2$, so

$$
\frac{d\theta}{(2-\cos\theta)^2}
=\frac4i\frac{z\,dz}{(z^2-4z+1)^2}.
$$

Write $r=2-\sqrt3$ and $s=2+\sqrt3$. Only $r$ lies inside the [unit circle](../../../../complex-unit-circle.md); the [rational function](../../../../rational-function.md) $h(z)=z/[(z-r)^2(z-s)^2]$ has a double [pole](../../../../pole.md) there. Its [residue](../../../../residue.md) is

$$
\operatorname{Res}_{z=r}h
=\left.\frac{d}{dz}\frac{z}{(z-s)^2}\right|_{z=r}
=\frac1{(r-s)^2}-\frac{2r}{(r-s)^3}
=-\frac{r+s}{(r-s)^3}=\frac1{6\sqrt3}.
$$

By the [residue theorem](../../../../residue-theorem.md),

$$
\boxed{\int_0^{2\pi}\frac{d\theta}{(2-\cos\theta)^2}
=\frac4i\,2\pi i\frac1{6\sqrt3}=\frac{4\pi}{3\sqrt3}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [6](../../6.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
