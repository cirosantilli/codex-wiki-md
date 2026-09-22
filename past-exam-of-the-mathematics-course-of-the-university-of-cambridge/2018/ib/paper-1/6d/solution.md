<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

Substituting the exact solution and expanding about $t_n$ gives the [local truncation error](../../../../../local-truncation-error.md)

$$
y(t_{n+1})-y(t_n)-\frac h2\bigl(y'(t_n)+y'(t_{n+1})\bigr)
=-\frac{h^3}{12}y'''(t_n)+O(h^4).
$$

Thus the method is consistent of order two; as a stable one-step method it has **global convergence order $k=2$**.

The order cannot be higher. For $y'=t^2$, $y(0)=0$, the exact solution is $y=t^3/3$, and direct substitution makes the local truncation error exactly

$$
\boxed{-\frac16h^3.}
$$

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
