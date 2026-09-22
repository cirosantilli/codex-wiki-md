<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep the original four-node [interpolation polynomial](../../../../../../interpolation-polynomial.md) $p$. The correction must vanish at all four original nodes, so a degree-at-most-four interpolant has the form

$$
q(x)=p(x)+c(x+1)x(x-1)(x-3).
$$

Since $p(2)=-1$ and the product at $2$ is $-6$, matching the new value gives $-1-6c=-7$, hence $c=1$. Expanding yields

$$
\boxed{q(x)=x^4-2x^3-3x^2+4x-3.}
$$

It takes the values $-7,-3,-3,-7,9$ at the five nodes. The same root-count argument proves uniqueness of this [interpolation polynomial](../../../../../../interpolation-polynomial.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
