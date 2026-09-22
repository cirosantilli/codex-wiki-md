<h1 id="9a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\epsilon=l/R$ and $a=1-\cos\theta_0$. Then

$$
\frac{r_B}{R}=\left(1+2a\epsilon+2a\epsilon^2\right)^{1/2}.
$$

The [binomial series](../../../../../../binomial-series.md) gives

$$
\frac{R}{r_B}=1-a\epsilon+\left(\frac32a^2-a\right)\epsilon^2+O(\epsilon^3),
$$

so

$$
v_2^2=2gR\left[a\epsilon+\left(a-\frac32a^2\right)\epsilon^2+O(\epsilon^3)\right].
$$

Since $v_1^2=2gRa\epsilon$, a second [binomial series](../../../../../../binomial-series.md) expansion yields

$$
\frac{v_2}{v_1}=1+\frac12\left(1-\frac32a\right)\epsilon+O(\epsilon^2)
=1+\left(-\frac14+\frac34\cos\theta_0\right)\frac lR+O\!\left(\frac{l^2}{R^2}\right).
$$

Thus the constants in the stated [Big O notation](../../../../../../big-o-notation.md) expansion are

$$
\boxed{A=-\frac14,\qquad B=\frac34}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9A](../../9a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
