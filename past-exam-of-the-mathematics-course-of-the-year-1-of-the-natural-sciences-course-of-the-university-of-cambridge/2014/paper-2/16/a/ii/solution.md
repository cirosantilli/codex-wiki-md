<h1 id="16/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrate the normal component on each face directly, with outward normals. Each unlisted pair of coordinates ranges independently from zero to one:

$$
\begin{array}{c|c|c}
\text{face}&\mathbf v\cdot\mathbf n&\text{flux}\\\hline
x=0&0&0\\
x=1&2(y+z)&2\\
y=0&-x^2&-1/3\\
y=1&x^2-1&-2/3\\
z=0&-y^2&-1/3\\
z=1&y^2-1&-2/3
\end{array}
$$

For example, on $x=1$ the [integral](../../../../../../integral-split.md) is $\int_0^1\int_0^1 2(y+z)\,dy\,dz=2$. Adding all six contributions gives

$$
\boxed{\int_{\partial V}\mathbf v\cdot d\mathbf S=0}.
$$

This calculation uses the six explicit [surface integrals](../../../../../../surface-integral.md), independently of the [divergence theorem](../../../../../../divergence-theorem.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [16](../../../16.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
