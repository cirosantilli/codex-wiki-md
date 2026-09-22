<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under the [Cameron-Martin theorem for a linear drift](../../../../../../../cameron-martin-theorem-for-a-linear-drift.md), the probability that Brownian motion with drift $-\mu$ reaches $x$ is

$$
\mathbb P(S\geq x)
=e^{-\mu x}\mathbb E\!\left[e^{-\mu^2T_x/2}\right].
$$

Using the supplied [Laplace transform](../../../../../../../laplace-transform.md) with $\lambda=\mu^2/2$ gives

$$
\mathbb E[e^{-\mu^2T_x/2}]=e^{-\mu x},
$$

and hence

$$
\mathbb P(S\geq x)=e^{-2\mu x}.
$$

This is the survival function of the [exponential distribution](../../../../../../../exponential-distribution.md) with rate $2\mu$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 201](../../../../paper-201-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
