<h1 id="1a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitution of $y_n=\lambda^n$ into the [linear recurrence relation](../../../../../../linear-recurrence-relation.md) gives $\lambda^n p(\lambda)=0$. Since $\lambda\ne0$, division by $\lambda^n$ proves **the sequence is a solution exactly when $p(\lambda)=0$**.

For a nonzero triple [root of a polynomial](../../../../../../root-of-a-polynomial.md) $\mu$, the [repeated characteristic root of a linear recurrence](../../../../../../repeated-characteristic-root-of-a-linear-recurrence.md) rule gives the three independent solutions $\mu^n,n\mu^n,n^2\mu^n$. One way to see the polynomial factors is to write $y_n=\mu^n z_n$: the recurrence becomes the third [forward difference operator](../../../../../../forward-difference-operator.md) applied to $z_n$ equal to zero, so $z_n$ is a quadratic [polynomial](../../../../../../polynomial-split.md). Thus

$$
\boxed{y_n=(A+Bn+Cn^2)\mu^n,\qquad \mu\ne0.}
$$

These three constants give arbitrary initial values $y_0,y_1,y_2$, hence the full third-order solution. If $\mu=0$, the recurrence instead reduces to $y_{n+3}=0$: **the first three values are arbitrary and every subsequent value is zero**. The nonzero-root formula must not be used to discard those initial values.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1A](../../1a.md)
3. [Section I](../../section-i.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
