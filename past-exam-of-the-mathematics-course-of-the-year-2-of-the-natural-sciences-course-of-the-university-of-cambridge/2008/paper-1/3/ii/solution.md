<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The zero initial value and slope select a forward [Green's function](../../../../../green-s-function-split.md): set it to zero for $x<\xi$, and choose the right piece to start at zero with slope one. This gives

$$
\boxed{G_2(x,\xi)=\begin{cases}0,&x\leq\xi,\\\tfrac12(x-\xi^2/x),&x\geq\xi.\end{cases}}
$$

For $f=1$ on $(0,1)$ and zero elsewhere,

$$
\boxed{y_2(x)=\begin{cases}x^2/3,&0<x\leq1,\\x/2-1/(6x),&x\geq1.\end{cases}}
$$

Indeed $y_2=\int_0^{\min(x,1)}(x-\xi^2/x)d\xi/2$. It and its first [derivative](../../../../../derivative.md) match at one, while $y_2,y_2'\to0$ at zero. The only homogeneous solution with these two initial limits is zero, so this solution too is unique. Its growth at infinity is allowed by these boundary conditions.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
