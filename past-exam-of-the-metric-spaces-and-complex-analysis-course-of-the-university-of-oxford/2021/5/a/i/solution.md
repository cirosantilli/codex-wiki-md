<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Start with the [partial fraction decomposition](../../../../../partial-fraction-decomposition.md)

$$
\frac1{(z+1)(z-2)}=-\frac1{3(z+1)}+\frac1{3(z-2)}.
$$

For $1<|z|<2$, expand the first fraction in negative powers and the second in nonnegative powers using the [geometric series](../../../../../geometric-series.md):

$$
\frac1{z+1}=\sum_{n=0}^\infty(-1)^nz^{-n-1},\qquad
\frac1{z-2}=-\sum_{n=0}^\infty\frac{z^n}{2^{n+1}}.
$$

Thus the [Laurent expansion](../../../../../laurent-series.md) on this [annulus](../../../../../annulus-mathematics.md) is

$$
\boxed{\frac1{(z+1)(z-2)}=-\frac13\sum_{n=0}^\infty(-1)^nz^{-n-1}-\frac13\sum_{n=0}^\infty\frac{z^n}{2^{n+1}},\qquad1<|z|<2.}
$$

For $|z|>2$, both fractions expand in negative powers:

$$
\frac1{z-2}=\sum_{n=0}^\infty2^nz^{-n-1}.
$$

Combining the two [geometric series](../../../../../geometric-series.md) gives

$$
\boxed{\frac1{(z+1)(z-2)}=\frac13\sum_{n=0}^\infty\bigl(2^n-(-1)^n\bigr)z^{-n-1},\qquad|z|>2.}
$$

The $z^{-1}$ coefficient is zero, consistently with the original [rational function](../../../../../rational-function.md) being $O(z^{-2})$ at infinity. Each displayed [series](../../../../../series-mathematics.md) converges absolutely on its stated [annulus](../../../../../annulus-mathematics.md) and uniformly on every [compact subset](../../../../../compact-space.md) of that [annulus](../../../../../annulus-mathematics.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [a](../../a.md)
3. [5](../../../5.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
