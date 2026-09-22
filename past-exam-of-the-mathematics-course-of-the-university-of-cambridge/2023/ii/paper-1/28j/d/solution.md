<h1 id="28j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the convention $J_0=0$, so $A(t)=t$ when $N_t=0$. Conditional on $N_t=n\geq1$, the last jump $J_n$ is the largest of $n$ independent uniform points on $[0,t]$. The stated [order statistic](../../../../../../order-statistic.md) formula gives

$$
\mathbb E(J_n\mid N_t=n)=\frac{nt}{n+1},
$$

and hence, for every $n\geq0$,

$$
\mathbb E(A(t)\mid N_t=n)=\frac{t}{n+1}.
$$

Putting $\mu=\lambda t$ and averaging over $N_t$,

$$
\begin{aligned}
\mathbb EA(t)
&=t e^{-\mu}\sum_{n=0}^\infty
\frac{\mu^n}{n!(n+1)}\\
&=t e^{-\mu}\frac{e^\mu-1}{\mu}\\
&=\boxed{\frac{1-e^{-\lambda t}}{\lambda}}.
\end{aligned}
$$

This agrees with [age of a Poisson process](../../../../../../age-of-a-poisson-process.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [28J](../../28j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
