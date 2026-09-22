<h1 id="5c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The identity

$$
(n+1)^3-2n^3+(n-1)^3=6n
$$

shows that $y_n^{(p)}=h^3n^3/6$ is a [particular solution](../../../../../../particular-solution.md). Combining it with the homogeneous solution from part (b) gives

$$
y_n=A+Bn+\frac{h^3n^3}{6}.
$$

The condition $y_0=0$ gives $A=0$, and $y_{-1}=y_1$ gives $B=-h^3/6$. Hence

$$
y_n=\frac{h^3}{6}(n^3-n).
$$

The exact initial-value solution is $y(t)=t^3/6$. Since $N=1/h$,

$$
y_N=\frac{1-h^2}{6},
\qquad
y_N-y(1)=\boxed{-\frac{h^2}{6}}.
$$

**Thus the absolute endpoint error is $h^2/6$, consistent with the second-order [truncation error](../../../../../../truncation-error.md) of the centred scheme.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5C](../../5c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
