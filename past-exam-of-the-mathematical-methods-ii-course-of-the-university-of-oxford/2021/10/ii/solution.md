<h1 id="10/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $a>0$ and choose the outward [orientation](../../../../orientation-of-a-simplex.md). On the [sphere](../../../../sphere.md), $\mathbf n=(x,y,z)/a$, so $\mathbf F\cdot\mathbf n=(x^2+y^2+2z^2)/a=(a^2+z^2)/a$. In [spherical coordinates](../../../../spherical-coordinate-system.md), $z=a\cos\theta$ and $dS=a^2\sin\theta\,d\theta\,d\phi$. The direct [surface integral](../../../../surface-integral.md) is

$$
\begin{aligned}
\oiint_S\mathbf F\cdot\mathbf n\,dS
&=a^3\int_0^{2\pi}\!d\phi\int_0^\pi(1+\cos^2\theta)\sin\theta\,d\theta\\
&=2\pi a^3\left(2+\frac23\right)
=\boxed{\frac{16\pi a^3}{3}}.
\end{aligned}
$$

Independently, $\nabla\cdot\mathbf F=1+1+2=4$. Its [volume integral](../../../../volume-integral.md) over the ball is

$$
\iiint_V4\,dV=4\int_0^a r^2\,dr\int_0^\pi\sin\theta\,d\theta\int_0^{2\pi}d\phi
=\boxed{\frac{16\pi a^3}{3}}.
$$

The two calculations agree exactly with the [divergence theorem](../../../../divergence-theorem.md). The expression requested is a scalar [flux](../../../../flux.md) of a [vector field](../../../../vector-field.md), namely the [dot product](../../../../dot-product.md) with the directed [surface area element](../../../../surface-area-element.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [10](../../10.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
