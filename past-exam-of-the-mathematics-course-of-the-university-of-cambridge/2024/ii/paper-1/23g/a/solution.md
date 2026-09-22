<h1 id="23g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Tonelli's theorem and the triangle inequality give

$$
\begin{aligned}
\int_0^\infty |G(y)g(y)|\,dy
&\leq\int_0^\infty\int_0^\infty
 |F(x,y)g(y)|\,dx\,dy\\
&=\int_0^\infty\left(\int_0^\infty
 |F(x,y)g(y)|\,dy\right)dx.
\end{aligned}
$$

Applying [Holder inequality](../../../../../../holder-inequality.md) in the $y$ variable for each fixed $x$ yields

$$
\int_0^\infty |G(y)g(y)|\,dy
\leq
\int_0^\infty
\left(\int_0^\infty |F(x,y)|^p\,dy\right)^{1/p}
\|g\|_q\,dx,
$$

and $\|g\|_q\leq1$ gives the claimed inequality. This is the duality proof of the [Minkowski integral inequality](../../../../../../minkowski-integral-inequality.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23G](../../23g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
