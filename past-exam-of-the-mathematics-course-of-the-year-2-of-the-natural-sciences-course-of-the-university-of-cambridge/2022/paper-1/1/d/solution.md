<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Since $\mathbf F=\nabla\Omega$, its [divergence](../../../../../divergence.md) is the [Laplacian](../../../../../laplacian.md) of $\Omega$:

$$
\nabla\cdot\mathbf F=\nabla^2\Omega=6x+4z.
$$

The [divergence theorem](../../../../../divergence-theorem.md) changes the outward [flux](../../../../../flux.md) through the whole closed boundary into $I=\int_V(6x+4z)dV$. Rotational symmetry makes the $x$ term vanish. With $z=(u^2-v^2)/2$ and the [Jacobian determinant](../../../../../jacobian-determinant.md) from part (c),

$$
\begin{aligned}
I&=2\int_{-\pi}^{\pi}\int_0^1\int_0^v(u^2-v^2)uv(u^2+v^2)\,du\,dv\,d\phi\\
&=4\pi\int_0^1v\left[\frac{u^6}{6}-\frac{v^4u^2}{2}\right]_{u=0}^{u=v}dv\\
&=-\frac{4\pi}{3}\int_0^1v^7\,dv
=\boxed{-\frac\pi6}.
\end{aligned}
$$

Both the curved face and the top disk are included in this [surface integral](../../../../../surface-integral.md) through the [divergence theorem](../../../../../divergence-theorem.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
