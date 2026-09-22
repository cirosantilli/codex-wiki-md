<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md), the formula at $t=0$ reads $r_0=r_0$, with an empty sum. If it holds at time $t$, substitution into the recursion gives

$$
r_{t+1}=\beta\left(\beta^tr_0+\sum_{s=1}^t\beta^{t-s}\xi_s\right)+\xi_{t+1}
=\beta^{t+1}r_0+\sum_{s=1}^{t+1}\beta^{t+1-s}\xi_s.
$$

Thus [mathematical induction](../../../../../../mathematical-induction.md) proves

$$
\boxed{r_t=\beta^tr_0+\sum_{s=1}^t\beta^{t-s}\xi_s.}
$$

No restriction such as $|\beta|<1$ is needed for this finite-time identity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
