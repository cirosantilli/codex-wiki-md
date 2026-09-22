<h1 id="23f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the centered [Hardy-Littlewood maximal function](../../../../../../hardy-littlewood-maximal-function.md)

$$
M\theta(x)=\sup_{r>0}\frac1{2r}
\int_{x-r}^{x+r}\theta(t)\,dt.
$$

If $x>0$, choosing $0<r<x$ makes the whole interval lie in the positive half-line, so $M\theta(x)=1$. If $x=0$, every centered interval has exactly half its length in the positive half-line, so $M\theta(0)=1/2$.

If $x<0$, the average is zero for $r\leq-x$. For $r>-x$, it is

$$
\frac{x+r}{2r}
=\frac12+\frac{x}{2r}<\frac12,
$$

and these values tend to $1/2$ as $r\to\infty$. Hence

$$
M\theta(x)=
\begin{cases}
1,&x>0,\\
\frac12,&x\leq0.
\end{cases}
$$

For the uncentered maximal-function convention, intervals extending arbitrarily far to the right make the supremum equal to $1$ at every $x$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [23F](../../23f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
