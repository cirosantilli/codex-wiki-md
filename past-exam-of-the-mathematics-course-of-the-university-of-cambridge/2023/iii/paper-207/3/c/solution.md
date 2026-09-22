<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An illness episode ends at total rate $\gamma+\delta$, so its mean duration is

$$
\frac1{\gamma+\delta}=10\text{ days}.
$$

The probability that its terminating transition is fatal is $\delta/(\gamma+\delta)=0.1$. Therefore, in day units,

$$
\widehat\delta=0.01,
\qquad
\widehat\gamma=0.09.
$$

Starting healthy, the first infection time is exponential with rate $\lambda_z$. Hence

$$
1-e^{-30\lambda_1}=0.06,
\qquad
1-e^{-30\lambda_0}=0.01,
$$

and

$$
\widehat\lambda_1=-\frac{\log0.94}{30},
\qquad
\widehat\lambda_0=-\frac{\log0.99}{30},
\qquad
\widehat\beta=\log\frac{\widehat\lambda_1}{\widehat\lambda_0}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
