<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

Take the [unit normal](../../../../../unit-normal.md) to point outwards. The [divergence](../../../../../divergence.md) of the field is

$$
\nabla\cdot\mathbf F=(9x^2-2x)y+(3y^2-4y+1)x+2z.
$$

The [divergence theorem](../../../../../divergence-theorem.md) turns the closed [surface integral](../../../../../surface-integral.md) into a volume integral over $[0,1]^3$:

$$
\begin{aligned}
I&=\int_0^1\int_0^1\int_0^1
\left[(9x^2-2x)y+(3y^2-4y+1)x+2z\right]dx\,dy\,dz\\
&=(3-1)\frac12+\frac12(1-2+1)+1
=\boxed{2}.
\end{aligned}
$$

For a direct check of the [surface integral](../../../../../surface-integral.md), on $x=1$ the outward component is $F_x=2y$, contributing $\int_0^1\int_0^1 2y\,dy\,dz=1$. On $x=0$ it vanishes. On both $y=0$ and $y=1$, $F_y=x y(y-1)^2=0$. On $z=1$, $F_z=0$, whereas on $z=0$ the field component is $F_z=-1$ and the outward normal is $-\widehat{\mathbf z}$, giving a contribution $1$. The six face contributions are therefore $1,0,0,0,0,1$, again totaling **2**. The positive bottom-face contribution is a consequence of its outward orientation.

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
