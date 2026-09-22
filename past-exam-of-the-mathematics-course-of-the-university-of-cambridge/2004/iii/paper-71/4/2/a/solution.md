<h1 id="4/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Cox-de Boor recurrence](../../../../../../../cox-de-boor-recursion-formula.md). For unit knots the order-two hat is $L(u)=u$ on $[0,1]$, $L(u)=2-u$ on $[1,2]$, and zero elsewhere. The order-three [quadratic cardinal B-spline](../../../../../../../quadratic-cardinal-b-spline.md) is

$$
q(u)=\frac u2L(u)+\frac{3-u}{2}L(u-1)
=\begin{cases}
\tfrac12u^2,&0\le u\le1,\\
\tfrac34-(u-\tfrac32)^2,&1\le u\le2,\\
\tfrac12(3-u)^2,&2\le u\le3,\\
0,&\text{otherwise}.
\end{cases}
$$

Thus $N_j(t)=q(t-j)$. At $x_i=i+3/2$, the only possible arguments in its [support](../../../../../../../support.md) are $3/2$ and $1/2,5/2$ at neighboring indices. Their values give

$$
\boxed{N_j(x_i)=\begin{cases}\tfrac34,&j=i,\\\tfrac18,&|j-i|=1,\\0,&|j-i|\ge2.\end{cases}}
$$

Indices outside $1,\ldots,n$ are absent, so the first and last rows have just one neighboring nonzero value.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [4](../../../4.md)
4. [Paper 71](../../../../paper-71-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
