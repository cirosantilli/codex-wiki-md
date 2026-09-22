<h1 id="6/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For the [exponential distribution](../../../../../../exponential-distribution.md) with mean $\mu$, $f_A(t)=F_A(t)/\mu$ and $F_A(t)=e^{-t/\mu}$. Therefore

$$
\mathbb P(T_A<T_B)=\frac1\mu\int_0^\infty F_A(t)F_B(t)\,dt
=\frac{\mathbb E X}{\mu}.
$$

Since ties have probability zero, $\mathbb P(X=T_B)=1-\mathbb E X/\mu$. Taking [expected values](../../../../../../expected-value.md) in the definition of $U$ gives

$$
\boxed{\mathbb E U=\mathbb E X+\mu\mathbb P(X=T_B)
=\mathbb E X+\mu-\mathbb E X=\mu=\mathbb E T_A.}
$$

There is also an imputation interpretation. If A is observed first, $T_A=X$; if B censors A, [memorylessness of the exponential distribution](../../../../../../memorylessness-of-the-exponential-distribution.md) and [independence](../../../../../../independent-random-variables.md) imply that the remaining mean lifetime is $\mu$. Thus $U$ is the [conditional expectation](../../../../../../conditional-expectation.md) of $T_A$ given the observed minimum and censoring indicator. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives the same equality. This does not say that $U$ and $T_A$ have the same distribution.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
