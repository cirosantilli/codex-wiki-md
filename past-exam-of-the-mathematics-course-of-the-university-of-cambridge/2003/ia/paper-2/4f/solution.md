<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The transformation is strictly increasing on $0\le x<1$, has range $[0,\infty)$, and its inverse is $x=y/(y+3)$. Therefore the [cumulative distribution function](../../../../../cumulative-distribution-function.md) is

$$
\boxed{F_Y(y)=\begin{cases}0,&y<0,\\[2pt]\dfrac{y}{y+3},&y\ge0.\end{cases}}
$$

Differentiation gives the [probability density function](../../../../../probability-density-function.md)

$$
\boxed{f_Y(y)=\frac{3}{(y+3)^2}\ \ (y>0),\qquad f_Y(y)=0\ \ (y<0).}
$$

Its value at zero may be assigned arbitrarily without changing the distribution. There is no atom at zero or infinity. The expression is undefined at $X=1$, but that event has [probability](../../../../../probability.md) zero under the continuous [uniform distribution](../../../../../continuous-uniform-distribution.md), so any convention there leaves the law unchanged. Finally $\int_0^\infty3/(y+3)^2\,dy=1$, as required.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
