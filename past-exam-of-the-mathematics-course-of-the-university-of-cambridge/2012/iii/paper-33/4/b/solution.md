<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) gives

$$
\mathbb E e^{\lambda X_1}=\exp\left(-\lambda+\frac{\lambda^2}{2}\right).
$$

Independence of $X_{n+1}$ from $\mathcal F_n$ implies

$$
\mathbb E[e^{\lambda S_{n+1}}\mid\mathcal F_n]=e^{\lambda S_n}\exp\left(-\lambda+\frac{\lambda^2}{2}\right).
$$

Every exponential here is integrable. Thus the process is a [martingale](../../../../../../martingale-split.md) exactly when $-\lambda+\lambda^2/2=0$. Its two roots are $0$ and $2$, and the unique positive root is

$$
\boxed{\lambda=2.}
$$

The resulting [exponential martingale of a random walk](../../../../../../exponential-martingale-of-a-random-walk.md) is nonnegative and has [expectation](../../../../../../expected-value.md) $1$ at every finite time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
