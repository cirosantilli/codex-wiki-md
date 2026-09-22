<h1 id="16/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [divergence](../../../../../divergence.md) is

$$
\nabla\cdot\boldsymbol F=2(y+3)+2z=2y+2z+6.
$$

For the tetrahedral domain, convenient integration bounds are

$$
0\leq x\leq1,\qquad 0\leq y\leq1-x,\qquad
0\leq z\leq2(1-x-y).
$$

Consequently its [volume integral](../../../../../volume-integral.md) is

$$
I=\int_0^1\int_0^{1-x}\int_0^{2(1-x-y)}(2y+2z+6)\,dz\,dy\,dx.
$$

Putting $h=2(1-x-y)$, the inner [integral](../../../../../integral-split.md) is $(2y+6)h+h^2=(16-4x)(1-x-y)$. Therefore

$$
\begin{aligned}
I&=\int_0^1(16-4x)\frac{(1-x)^2}{2}\,dx\\
&=\int_0^1(8-18x+12x^2-2x^3)\,dx
=8-9+4-\frac12.
\end{aligned}
$$

Thus

$$
\boxed{I=\frac52.}
$$

There is an independent [centroid](../../../../../centroid.md) check. The vertices are $(0,0,0),(1,0,0),(0,1,0),(0,0,2)$, giving volume $1/3$ and centroid $(1/4,1/4,1/2)$. An [affine function](../../../../../affine-function.md) averages to its value at the centroid, so $I=(1/3)(6+2/4+2/2)=5/2$. This is the [integral of an affine function over a simplex](../../../../../integral-of-an-affine-function-over-a-simplex.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [16](../../16.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
