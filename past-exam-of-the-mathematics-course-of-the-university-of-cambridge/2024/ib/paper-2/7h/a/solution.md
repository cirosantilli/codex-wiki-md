<h1 id="7h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use multipliers $\lambda,\mu\geq0$ for

$$
x_1+x_2-c\leq0,
\qquad
\sqrt{x_2}-d\leq0.
$$

At an interior point in the nonnegative quadrant, the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) are

$$
\log x_1+1+\lambda=0,
$$



$$
-1+\lambda+\frac{\mu}{2\sqrt{x_2}}=0,
$$

with complementary slackness for the two constraints.

For $c=3/e^2$ and $d=2/e$, the square-root constraint is inactive at the answer, so $\mu=0$. The second stationarity equation gives $\lambda=1$, and the first gives $x_1=e^{-2}$. The sum constraint is active, hence

$$
\boxed{x_1=\frac1{e^2},
\qquad
x_2=\frac2{e^2}}.
$$

Indeed, $\sqrt{x_2}=\sqrt2/e<2/e$. The minimum value is

$$
\boxed{-\frac4{e^2}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7H](../../7h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
