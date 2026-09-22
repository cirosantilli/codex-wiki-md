<h1 id="19d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Evaluating the [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) coefficients at five, and their derivatives at one, gives

$$
\boxed{f(5)\approx f(0)-5f(2)+5f(3),\qquad
f'(1)\approx\frac{f(2)-f(0)}2.}
$$

Both rules are exact for every polynomial of degree at most two. For $f(x)=x^3$, the first gives $95$, while the true value is $125$; the second gives $4$, while the true derivative is $3$. Thus **the respective approximation errors, estimate minus true value, are $-30$ and $1$**. There is no contradiction: a cubic lies outside the exactness class. The first formula extrapolates beyond the interpolation nodes, so its error can be substantial.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19D](../../19d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
