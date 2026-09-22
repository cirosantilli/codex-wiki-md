<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Only reaction 1 changes $X_1$. Starting from five molecules, its successive states are $5\to3\to1$, with rates $5^2=25$ and $3^2=9$; state one is then absorbing for this channel. Thus

$$
\mathbb P(X_1(t)=5)=e^{-25t}.
$$

The probability of still being at three is the [convolution](../../../../../../convolution.md) of the first waiting time with an [exponential distribution](../../../../../../exponential-distribution.md) and survival of the second:

$$
\mathbb P(X_1(t)=3)
=\int_0^t25e^{-25s}e^{-9(t-s)}\,ds
=\frac{25}{16}\left(e^{-9t}-e^{-25t}\right).
$$

Applying the [law of total probability](../../../../../../law-of-total-probability.md) to the three possible states gives

$$
\boxed{g(t)=1-\frac{25}{16}e^{-9t}
+\frac9{16}e^{-25t}.}
$$

It has $g(0)=0$ and tends to one as both reaction waiting times elapse.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
